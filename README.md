## aitl-lab

## プロジェクト概要

本プロジェクト「aitl-lab」は、SoC制御系のPoC設計におけるAll-in-Theory Logic (AITL) 対応マニュアルおよび関連資産の体系的管理を目的としています。  
AITL理論を基盤に、制御系設計、RTL/ソフト連携、評価、SystemDK移行までの一連の設計プロセスを包括的に扱います。

## ディレクトリ構成
```
aitl-lab/
├── docs/                              # マニュアル・設計資料（Markdown形式）
│   ├── SoC_PoC_Manual_v5.0.md        # PoCマニュアル（中核ドキュメント）
│   ├── aitl-theory/                   # AITL理論関連ドキュメント
│   │    ├── overview.md               # AITL理論の概要説明
│   │    ├── concepts.md               # 主要概念・用語解説
│   │    └── examples.md               # 理論の具体例・ケーススタディ
│   ├── tutorial/                      # 教育・チュートリアル資料
│   │    ├── getting_started.md        # 入門ガイド
│   │    ├── poc_workflow.md           # PoC開発手順・実践例
│   │    └── tools_usage.md            # ツールの使い方
│   ├── references/                    # 参考資料、関連論文等
│   └── architecture/                  # AITL構造記述、SystemDK構成ファイル
├── src/                              # 実装コード・PoC
│   ├── rtl/                          # ハードウェア設計（Verilog/SystemVerilog）
│   └── sw/                           # ソフト制御コード（RISC-V等）
├── templates/                        # 設計テンプレート・フォーマット類
├── eval/                            # 評価データ・ログ
└── README.md
```

## 進行ルール

- 章ごとにMarkdownファイルへ追記し、バージョン管理を徹底  
- ソースコードは機能単位で分割し、`src/rtl/` と `src/sw/` で管理  
- ドキュメントは `docs/` 以下に一元化し、テンプレート利用を推奨  
- SystemDK移行対応は `docs/architecture/` および `src/ip/` を参照  
- 評価は `eval/` に記録し、定期的に結果共有とレビューを実施

## 貢献方法

- 新規機能追加や修正は、ブランチを切ってPull Requestで提案してください  
- ドキュメント修正は内容の正確性と表現の明瞭性を重視  
- コード修正は動作確認と簡易テストの実施を必須とします

## 連絡先

- プロジェクト管理者: 三溝 真一  
- GitHubリポジトリ: https://github.com/aitl-lab  
- 問い合わせ: issue登録またはメールでご連絡ください

## ライセンス

本プロジェクトのソースコードおよびドキュメントはMITライセンスのもと公開しています。  
詳細はLICENSEファイルを参照してください。
