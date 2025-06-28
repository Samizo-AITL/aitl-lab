# 付録A：設計テンプレート・PoC成果記録フォーマット

## A.1 設計テンプレートの目的

PoC設計において、情報の記録・再利用性を高め、チーム内での認識共有を円滑にするための設計テンプレートを提供する。

---

## A.2 テンプレート一覧

| テンプレート名 | 概要 | 格納先 |
|----------------|------|--------|
| `spec_template.md` | PoC仕様書テンプレート | `templates/` |
| `module_design.md` | 各モジュール設計記述用 | `templates/` |
| `eval_log_format.csv` | 評価ログ記録用CSV | `eval/` |
| `ip_register_map.xlsx` | IPレジスタマップ管理用 | `templates/` |
| `risk_checklist.md` | 設計リスクチェックリスト | `templates/` |

---

## A.3 記録フォーマット例：PoC成果記録

```markdown
# PoC成果記録（例）

- 日付: YYYY-MM-DD
- モジュール名: xyz_controller
- 担当: 三溝
- 実施内容: シミュレーション評価実施（パターン3）
- 結果: 正常動作、出力信号一致（詳細は eval/log_xyz_2025xxxx.csv）
- 課題: クロックジッタに対するマージン低め、改善予定
- コメント: バージョンv0.9のまま次フェーズへ移行見込み
```
