# SeedMind Architecture — Components

---

## 日本語

このドキュメントは、SeedMindアーキテクチャを構成する  
主要コンポーネントの**責務（responsibility）**を定義する。

ここで定義されるコンポーネントは、  
具体的なクラス、モジュール、実装単位を示すものではない。  
SeedMindの思想を成立させるために必要な  
**役割としての構成要素**を示すものである。

各コンポーネントは独立した責務を持ちながら、  
Decisionを中心とした循環構造の一部として機能する。

---

## English

This document defines the **responsibilities** of the core components  
that constitute the SeedMind architecture.

The components described here do not correspond to concrete classes,  
modules, or implementation units.  
They represent **conceptual roles** required to sustain the SeedMind framework.

Each component has an independent responsibility  
while functioning as part of a decision-centric loop.

---

## Core Components

### Self Model

#### 日本語
SeedMind自身の状態、制約、傾向、価値観を表現する内部モデル。

- 自己を参照するための基準点となる  
- 判断の一貫性を保つために利用される  
- 外部から直接操作されることはない  

Self Modelは固定された設定ではなく、  
経験とEvolutionを通じて更新される。

#### English
An internal model representing SeedMind’s state, constraints, tendencies, and values.

- Serves as a reference point for self-awareness  
- Maintains consistency in decision-making  
- Not directly manipulated by external systems  

The self-model is not static and evolves through experience.

---

### Memory

#### 日本語
過去の経験、知識、学習結果を保持する構造。

- 保存そのものが目的ではない  
- 将来のDecisionに影響を与えるために存在する  
- 参照されない記憶は意味を持たない  

Memoryは静的なデータストアではなく、  
行動を変化させるための構造として扱われる。

#### English
A structure that holds past experiences, knowledge, and learned outcomes.

- Exists to influence future decisions, not merely to store data  
- Memory without reference has no functional meaning  

Memory is treated as a behavior-shaping structure rather than a static datastore.

---

### Interpretation

#### 日本語
外部入力を内部で扱える形式へ変換するコンポーネント。

- 入力の正規化  
- 文脈や構造の抽出  
- 判断に必要な情報の整理  

Interpretationは意味を整形するが、  
行動の選択には関与しない。

#### English
Transforms external input into an internally usable representation.

- Normalization  
- Context and structure extraction  
- Information organization for decision-making  

Interpretation structures meaning but does not select actions.

---

### Decision Engine

#### 日本語
SeedMindの中核となる判断コンポーネント。

- Self Model と Memory を参照する  
- 行動・応答・沈黙を含む選択を行う  
- 常に何らかの結果を返す  

Decision Engineは出力生成ではなく、  
**行動選択そのもの**を責務とする。

#### English
The central decision-making component of SeedMind.

- References the Self Model and Memory  
- Selects actions, responses, or silence  
- Always produces a decision outcome  

Its responsibility is action selection, not output generation.

---

### Expression

#### 日本語
Decisionで選択された内容を、  
外部に伝達可能な形式へ変換するコンポーネント。

- 発話や応答形式の生成  
- 表現スタイルの調整  

ExpressionはDecisionの結果を表現するが、  
判断そのものは行わない。

#### English
Converts decisions into externally communicable forms.

- Generates speech or response formats  
- Adjusts expression style  

Expression represents decisions but does not decide.

---

### Action

#### 日本語
外部環境に対して実際の影響を与えるコンポーネント。

- ツールの呼び出し  
- システム操作  
- 状態変更の実行  

ActionはExpressionと分離される場合もあるが、  
どちらもDecisionの結果として扱われる。

#### English
Executes concrete effects on the external environment.

- Tool invocation  
- System operations  
- State changes  

Action may be separated from Expression but is always a result of Decision.

---

### Reflection

#### 日本語
行動や応答の結果を評価するコンポーネント。

- 結果の観測  
- 意図との比較  
- 内部構造への影響評価  

Reflectionは即時または遅延して行われる。

#### English
Evaluates the outcomes of actions or responses.

- Observes results  
- Compares outcomes with intent  
- Assesses impact on internal structures  

Reflection may occur immediately or asynchronously.

---

### Evolution

#### 日本語
SeedMindの内部構造を更新するコンポーネント。

- Memoryの更新  
- Self Model の調整  
- 判断基準の変化  

Evolutionにより、  
同一の入力に対して異なるDecisionが可能となる。

#### English
Updates SeedMind’s internal structures.

- Memory updates  
- Self-model adjustments  
- Decision criteria changes  

Through evolution, identical inputs may yield different decisions over time.

---

## Design Notes

### 日本語
- 各コンポーネントは単一責務を持つ  
- Decisionは常に中核に存在する  
- 学習は外部処理ではなく内部循環として扱われる  
- 実装上の統合や分割は自由である  

### English
- Each component has a single responsibility  
- Decision remains the central core  
- Learning is treated as an internal loop  
- Implementation-level composition is flexible  

---

## Positioning

### 日本語
このコンポーネント定義は、  
SeedMindアーキテクチャにおける責務分解の基準を示す。

具体的な実装やアルゴリズムはここでは規定しない。

### English
This component definition provides a responsibility-based decomposition  
for the SeedMind architecture.

Concrete implementations and algorithms are intentionally unspecified.
