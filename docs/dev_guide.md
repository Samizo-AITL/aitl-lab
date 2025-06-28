# AITL PoC 開発ガイド

このドキュメントは、AITL制御PoCの内部構造・拡張方法・コーディングルールを開発者向けにまとめたものです。

---

## 🗂 ディレクトリ構成

PoCは以下のような構成で整理されています：

\```
poc/
├── control/        # 制御ロジック（AITL, PID, etc.）
├── sim/            # シミュレータ（物理モデル）
├── config/         # 実行設定ファイル（YAML形式）
├── ui/             # UI/グラフ描画モジュール（任意）
├── logs/           # 実行ログ出力（JSONなど）
├── main.py         # エントリーポイント（PoC起動）
└── utils/          # 共通関数・補助モジュール
\```

---

## ⚙️ モジュールの役割

### control/

AITL方式をはじめ、さまざまな制御方式を実装するディレクトリです。

- `aitl_control.py`：AITL理論に基づく制御ロジック
- `pid_control.py`：一般的なPID制御（比較用）

インターフェース（例）：

```python
output = controller.update(state, target)
```

### sim/

物理システム（例：2次元リンク、慣性モデル）を定義。

- `plant_model.py`：物理方程式ベースのモデル
- `state_update.py`：状態の時間発展ロジック

### config/

- 実験パラメータ、初期状態、制御方式などをYAMLで記述。

### ui/

- matplotlibなどによる結果可視化、リアルタイム表示を含む

---

## 🔁 実行の流れ

```
main.py
├── 設定読み込み（config/）
├── シミュレータ初期化（sim/）
├── 制御器セットアップ（control/）
├── ループ実行（時間発展）
└── ログ保存・UI描画（logs/, ui/）
```

---

## ➕ 拡張方法

### 1. 新しい制御方式の追加

`control/your_method.py` を作成し、以下の形式を満たす：

```python
class YourController:
    def __init__(self, config):
        ...
    def update(self, state, target):
        return control_output
```

`main.py` に以下を追記：

```python
if control_type == "YourMethod":
    controller = YourController(config)
```

### 2. 新しい物理モデルの追加

- `sim/` に `new_model.py` を追加し、`step(state, control)` 関数を定義。
- `main.py` から分岐呼び出し可能にする。

---

## 🧑‍💻 コーディング指針（任意）

- ファイル名・関数名はスネークケース（例：`step_simulation`）
- コントローラは `update()` を標準インターフェースとする
- ログ出力は `logs/` にJSON形式で統一
- UI表示はオプション：結果確認に依存しない構造にする

---

## 🔗 関連ドキュメント

- [overview.md](./overview.md)：このPoCの背景と目的  
- [usage.md](./usage.md)：基本的な使い方

---

## 📘 中核マニュアル

本PoCの理論的背景と制御アルゴリズムの詳細は、以下をご覧ください：

- [SoC_PoC_Manual_v5.0.md](./SoC_PoC_Manual_v5.0.md)
- 
