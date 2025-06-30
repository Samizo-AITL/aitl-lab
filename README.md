# AITL-Lab: AITL制御PoCリポジトリ

**AITL-Lab** は、AITL（All-in-Theory Logic）理論に基づく **制御PoC** および **AIアーキテクチャ開発** のための統合リポジトリです。

- 🧠 **AITL理論**：推論・制御・物理制約を統合的に捉えるAI設計思想  
- 🛠 **本リポジトリ**：理論に基づいたソフト・ハード一体の実装／評価環境  
- 🎓 **対象**：AI・制御・ロボティクス・半導体・組込み分野の研究者、教育者、技術者

---

## 📂 ディレクトリ構成（概要）
```
aitl-lab/
├── docs/
│   ├── SoC_PoC_Manual_v5.0.md               # 制御PoCの中核マニュアル
│   ├── soc-manual/                          # AITL SoC設計マニュアル（統合設計編）
│   │   └── AITL_SoC_Design_Manual_v1.0.md   # AITL構想に基づくSoC統合設計ドキュメント
│   ├── aitl-theory/                         # 理論ドキュメント（概念・用語・応用）
│   ├── tutorial/                            # 入門・チュートリアル
│   ├── references/                          # 関連文献・資料
│   └── architecture/                        # AITL構造・SystemDK関連
├── src/                  # 実装コード（PoC実験）
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
| 📘 [`SoC_PoC_Manual_v5.0.md`](./docs/SoC_PoC_Manual_v5.0.md) | 制御PoCの中核マニュアル |
| 🛠 [`soc-manual/AITL_SoC_Design_Manual_v1.0.md`](./docs/soc-manual/AITL_SoC_Design_Manual_v1.0.md) | AITL構想に基づくSoC実装マニュアル（設計・統合編） |
| 🧠 [`aitl-theory/`](./docs/aitl-theory/) | 理論概要・用語集・応用事例 |
| 🎓 [`tutorial/`](./docs/tutorial/) | 入門・開発手順・ツール解説 |
| 📚 [`references/`](./docs/references/) | 関連論文・参考資料 |
| 🏗 [`architecture/`](./docs/architecture/) | AITL構造記述・SystemDK関連資料 |

---

## 📌 AITLとは？

**AITL（All-in-Theory Logic）** は、知能制御システムを理論的・構造的に設計することを目的とした**AIアーキテクチャ構想**です。

- 推論・制御・物理情報を3層に分離しつつ、統合的に扱う設計論理  
- モデルベース開発とAI推論を連携させた構造  
- ソフトウェアとハードウェア（SoC）を包含した設計手法（SystemDK準拠）

---

## 🧪 ライセンス・利用

- **ライセンス**：MIT（コード・ドキュメントとも）  
- **利用形態**：個人・教育・研究用途での利用を歓迎  
- **注意事項**：再利用時は必ず出典を明記してください

---

## 🙋‍♂️ 貢献・連絡先

- バグ報告・改善提案は [GitHub Issues](https://github.com/Samizo-AITL/aitl-lab/issues) へ  
- 技術ディスカッションは Discussions または関連リポジトリへ投稿歓迎

---

## 🔗 関連リポジトリ

- [`theory`](https://github.com/Samizo-AITL/theory)：AITL理論の抽象化・設計言語モデル  
- [`edusemi`](https://github.com/Samizo-AITL/edusemi)：半導体・制御系基礎教材
- 
