# AITL-Lab: AITL制御PoCリポジトリ

AITL-Lab は、AITL（All-in-Theory Logic）理論に基づく**制御PoC**および**AIアーキテクチャ開発**のための統合リポジトリです。

- 🧠 **AITL理論**：推論・制御・物理制約を統合的に捉えるAI設計思想  
- 🛠 **本リポジトリ**：理論に基づいたソフト・ハード一体の実装／評価環境  
- 🎓 **対象**：AI・制御・ロボティクス・半導体・組込み分野の研究者、教育者、技術者

---

## 📂 ディレクトリ構成（概要）

```
aitl-lab/
├── docs/                 # マニュアル・設計資料（Markdown形式）
│   ├── SoC_PoC_Manual_v5.0.md       # 中核マニュアル
│   ├── aitl-theory/                 # 理論ドキュメント（概念・例・概要）
│   ├── tutorial/                    # 入門・チュートリアル
│   ├── references/                  # 関連文献・資料
│   └── architecture/                # AITL構造・SystemDK
├── src/                  # 実装コード一式（PoC）
│   ├── rtl/              # RTL設計（Verilog等）
│   └── sw/               # ソフトウェア制御（RISC-Vなど）
├── templates/            # 設計テンプレート・書式類
├── eval/                 # 評価結果・ログ・グラフ
└── README.md             # 本ファイル
```

---

## 🚀 クイックスタート（PoC実行）

PoC動作確認用の簡易実行手順：

```bash
cd src/sw/poc
pip install -r requirements.txt
python main.py
```

詳細は `docs/tutorial/getting_started.md` および `docs/SoC_PoC_Manual_v5.0.md` を参照。

---

## 📖 ドキュメント案内

| 種別 | 内容 |
|------|------|
| 📘 [SoC_PoC_Manual_v5.0.md](./docs/SoC_PoC_Manual_v5.0.md) | 制御PoCの中核マニュアル |
| 🧠 [aitl-theory/](./docs/aitl-theory/) | 理論概要・概念・ケーススタディ |
| 🎓 [tutorial/](./docs/tutorial/) | 入門・開発手順・ツール使い方 |
| 📚 [references/](./docs/references/) | 関連論文・参考資料 |
| 🏗 [architecture/](./docs/architecture/) | AITL構造・SystemDK定義など |

---

## 📌 AITLとは？

AITL（All-in-Theory Logic）は、**知能制御システムを理論的・構造的に設計**することを目的としたAIアーキテクチャ構想です。  
特徴：

- 制御・推論・物理情報を一体で扱う構造
- ソフト＋ハードの両面を想定（SystemDK/SoCレベルまで）

---

## 🧪 ライセンス・利用

- ライセンス：MIT（コード・ドキュメントとも）  
- 個人・教育・研究用途での利用を歓迎します  
- 再利用の際は出典明記をお願いします

---

## 🙋‍♂️ 貢献・連絡先

- バグ報告・改善提案は GitHub Issues へ  
- 技術的なディスカッションは Discussions または別リポジトリへ

---

## 🔗 関連リポジトリ

- [`theory`](https://github.com/Samizo-AITL/theory)：AITL理論の抽象化・設計言語モデル
- [`edusemi`](https://github.com/Samizo-AITL/edusemi)：半導体・制御系基礎教材
