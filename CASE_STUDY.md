# 環境時系列データの再解析 / Environmental Time-Series Reanalysis

[紹介ページを開く / Open the presentation page](https://kelly-wk.github.io/environmental-timeseries/)

> **再解析設計修復済み・数値結果非公開 / Reanalysis design repaired · numeric results withheld**  
> 公開ケーススタディ / Public case study

## 概要 / Overview

重複窓による擬似反復を避け、依存性を考慮した介入時系列へ再設計した監査研究。

An audited reanalysis replacing overlapping-window pseudo-replication with dependence-aware interrupted time-series methods.

## 主なポイント / Highlights

1. **重複移動窓を独立標本として扱う誤った仮定を特定。**  
   Identified the invalid assumption that overlapping moving windows were independent samples.
2. **日次系列を直接モデル化し、HAC・AR(1)・移動ブロック法で依存性を反映。**  
   Modeled the daily series directly and represented dependence with HAC, AR(1), and moving-block methods.
3. **代替仕様を保持し、観察時系列から因果効果を断定しない報告へ修正。**  
   Retained alternative specifications and revised the report to avoid causal claims from an observational series.

## 研究の流れ / Research Flow

| 段階 / Stage | 内容 / Evidence |
|---|---|
| **課題 / Problem** | 重複窓と系列相関によって過小評価された不確実性を修正する。<br>Correct uncertainty that was understated by overlapping windows and serial correlation. |
| **方法 / Method** | 日次データの介入時系列にHAC、AR(1)、移動ブロックブートストラップを適用する。<br>Apply HAC, AR(1), and moving-block bootstrap methods to a daily interrupted time series. |
| **検証 / Validation** | ラグと仕様を変えた感度分析で、推定の方向と不確実性の依存を確認する。<br>Use lag and specification sensitivity analyses to assess dependence of direction and uncertainty. |
| **成果 / Outcome** | 独立性を仮定した元解析を、依存性を明示する再解析設計へ置き換えた。<br>Replaced the independence-based original analysis with an explicitly dependence-aware design. |

## 使用手法 / Methods

R, Interrupted time series, HAC covariance, AR(1) errors, Moving-block bootstrap, Lag analysis

## 限界と適用範囲 / Limitations & Scope

- 授業由来の原データは公開権限が未確認で、介入後期間も短いため因果解釈はできない。  
  Publication rights for the course-supplied raw data are unconfirmed, and the short post-intervention period precludes causal interpretation.

## 公開範囲 / Publication Boundary

公開ページは再解析設計と監査上の学びのみ。原データの利用・再配布許諾が未確認のため、コード、図表、数値結果は公開しない。

The public page covers only the repaired analysis design and audit lessons. Code, figures, and numeric results remain private because permission to use and redistribute the source data is unconfirmed.

---

この文書は公開可能な範囲だけで構成されています。  
This document contains only material cleared for public presentation.
