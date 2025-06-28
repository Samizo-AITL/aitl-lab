# AITL PoC 使用方法

このドキュメントでは、AITL制御PoC（Proof of Concept）のセットアップ方法と、基本的な実行手順を説明します。

---

## 🔧 必要な環境

AITL PoCは、Pythonベースのシミュレーション制御環境です。以下の環境で動作を確認しています。

- Python 3.9 以上  
- OS：macOS / Linux / Windows（WSL 推奨）  
- 仮想環境（推奨）：venv または conda  

---

## 📦 ライブラリのインストール

まず、必要なPythonライブラリをインストールします。

```bash
pip install -r requirements.txt
```

---

## 🚀 実行手順（基本）

このPoCは、Python環境上で簡単に動作確認ができます。以下の手順で実行してください。

### 1. 実行ディレクトリに移動

```bash
cd aitl-lab/poc/
```

### 2. メインスクリプトの実行

```bash
python main.py
```

これにより、指定された制御ロジックとシミュレータが連動して動作を開始し、結果が出力されます。

---

## ⚙️ 設定ファイルの編集（config.yaml）

PoCの動作は `config/config.yaml` ファイルで柔軟に設定できます。  
たとえば、以下のような項目があります：

```yaml
control_type: AITL-Logic
initial_state: [0.0, 0.0]
target_state: [1.0, 1.0]
time_step: 0.05
duration: 10.0
```

### 主なパラメータの説明

| パラメータ       | 内容                                   |
|------------------|----------------------------------------|
| control_type     | 使用する制御方式（例：AITL-Logic, PID）|
| initial_state    | 初期状態ベクトル（出発点）             |
| target_state     | 目標状態ベクトル（到達すべき点）       |
| time_step        | シミュレーションの刻み幅（秒）         |
| duration         | シミュレーション全体の長さ（秒）       |

---

## 📈 実行結果の確認方法

PoCの実行後、以下のような成果物が生成されます。

### ログファイル（logs/ ディレクトリ）

- 制御出力・状態遷移・誤差などが記録されます。
- 例：`logs/last_run.json`

### グラフ可視化（自動 or 手動）

- `matplotlib` によるグラフ出力。
- `poc/ui/plot_result.py` などを使って描画も可能。

### UI表示（オプション）

- `ui/` モジュールが有効な構成ならリアルタイム描画可能。
- Tkinter や PyQt などの追加インストールが必要な場合あり。

---

## 🛠 トラブルシューティング

| 問題                         | 対処法                                                   |
|------------------------------|-----------------------------------------------------------|
| ModuleNotFoundError が出る   | `PYTHONPATH` を設定 or VSCodeのワークスペース設定       |
| 実行後に何も表示されない     | `config.yaml` の `duration` や `target_state` を確認     |
| グラフが表示されない         | `matplotlib` のインストール確認 (`pip install matplotlib`) |

---

## 🔗 関連ドキュメント

- [overview.md](./overview.md)：このPoCの目的や構成  
- [dev_guide.md](./dev_guide.md)：内部構造と開発ルールの詳細  

---

## 📘 中核マニュアル

本PoCの理論的背景と制御アルゴリズムの詳細は、以下をご覧ください：

- [SoC_PoC_Manual_v5.0.md](./SoC_PoC_Manual_v5.0.md)
