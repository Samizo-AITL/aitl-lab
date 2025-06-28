# AITL PoC 概要

## 🧠 AITLとは？

AITL（All-in-Theory Logic）は、AIシステムを以下の3つの視点から設計するための理論構想です：

- **推論（Inference）**
- **制御（Control）**
- **物理的制約（Physics-informed Constraints）**

AITLでは、知能システムを論理的かつ構造的に組み立て、現実世界の動作と整合性の取れたAIを目指します。

---

## 🎯 このPoCの目的

このPoC（Proof of Concept）は、AITLの理論を以下のような形で実際に試すための「実験環境」です。

- 制御理論をベースにしたAIモデルを構築する
- 物理シミュレータ上で制御の動作を観察する
- AITL理論の設計指針を確認・改善する

---

## 🧩 構成要素（モジュール）

このPoCには、以下のようなモジュールが含まれます：

- **制御ロジック（control/）**：AITL方式の制御アルゴリズム
- **シミュレータ（sim/）**：動作確認用の物理モデル（例：2軸アーム）
- **UI表示（ui/）**：動作状態を可視化（任意）
- **設定ファイル（config/）**：制御方式や初期条件の定義

---

## 📚 関連ドキュメント

- [`usage.md`](./usage.md)：このPoCの動かし方
- [`dev_guide.md`](./dev_guide.md)：開発者向けの構造説明
- [`SoC_PoC_Manual_v5.0.md`](./SoC_PoC_Manual_v5.0.md)：制御PoCの中核マニュアル
