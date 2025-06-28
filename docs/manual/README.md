# PoCマニュアル（v5.0）目次案内

このディレクトリ `docs/manual/` は、AITL構想に基づく SoC制御系 PoC 設計に関する中核ドキュメントである  
**SoC_PoC_Manual_v5.0.md** を章別に構造化したものです。  
基礎から応用、実装・評価、SystemDK移行、出口戦略まで、段階的に構成されています。

---

## 📘 章構成（本編）

| 章番号 | ファイル名 | 概要 |
|--------|------------|------|
| 0 | `chapter00_intro.md` | マニュアルの目的と全体像 |
| 1 | `chapter01_spec_definition.md` | 仕様策定と要件定義（AITL視点） |
| 2 | `chapter02_control_design.md` | 制御系設計の実務ポイント |
| 3 | `chapter03_rtl_design.md` | RTL設計におけるAITL対応 |
| 4 | `chapter04_pdk_foundry.md` | PDK・ファウンドリ選定 |
| 5 | `chapter05_sw_collaboration.md` | ソフト設計とAITL連携 |
| 6 | `chapter06_sensor_if.md` | センサ混載とアナログIF設計 |
| 7 | `chapter07_dft.md` | DFTとテスト容易化 |
| 8 | `chapter08_self_repair.md` | AI自己修復PoC設計 |
| 9 | `chapter09_soc_integration.md` | SoC統合と協調設計 |
| 10 | `chapter10_project_management.md` | プロジェクト管理とAITL評価体系 |
| 11 | `chapter11_exit_strategy_systemdk.md` | 出口戦略とSystemDK移行設計 |
| 12 | `chapter12_poc_evaluation_management.md` | 評価指標とプロジェクト管理（再整理） |
| 13 | `chapter13_physical_verification.md` | 物理・実装検証 |
| 14 | `chapter14_device_interface.md` | 外付け・混載デバイスとのIF設計 |
| 15 | `chapter15_systemdk_ip_restructuring.md` | SystemDK移行とIP再構成 |
| 16 | `chapter16_exit_strategies.md` | 出口戦略別SystemDK方針 |

---

## 📎 付録

| 付録 | ファイル名 | 内容 |
|------|------------|------|
| A | `appendix_a_templates.md` | 設計テンプレート・成果記録フォーマット |
| B | `appendix_b_exit_checklist.md` | 出口戦略別チェックリスト |
| C | `appendix_c_poc_to_systemdk.md` | PoCDK→SystemDK変換事例集 |

---

## 📚 関連ディレクトリへのリンク

- [aitl-theory/](../aitl-theory/) … AITL理論の基礎資料（用語・構造・概念）
- [tutorial/](../tutorial/) … 実装手順やチュートリアル（実装者向けガイド）
- [SoC_PoC_Manual_v5.0.md](../SoC_PoC_Manual_v5.0.md) … 本マニュアルの統合版（一括版）

---

## 📌 注意事項

- 本マニュアルは随時更新中です。章・付録に未完成部分がある可能性があります。
- ご意見・改善提案は GitHub Issue にて歓迎します。
