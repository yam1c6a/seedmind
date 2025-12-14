# SeedMind Architecture — Overview

---

## 日本語

このドキュメントは、SeedMindアーキテクチャの全体構造を示す。  
ここで定義される構造は、実装の都合による分割ではなく、SeedMindの思想を成立させるための責務分離を目的としている。

SeedMindのアーキテクチャは、**意思決定を中心に、自己モデルと記憶が循環する構造**として設計されている。  
各レイヤは独立した責務を持ちつつ、単一の知性として一貫した振る舞いを実現するために連携する。

---

## English

This document describes the overall structure of the SeedMind architecture.  
The structure defined here is not a decomposition for implementation convenience, but a responsibility separation required to sustain the SeedMind concept.

SeedMind is designed as a **decision-centric loop** where a self-model and memory continuously inform action selection.  
Each layer has an independent responsibility while cooperating to behave as a single coherent intelligence.

---

## Core Cycle

### 日本語
SeedMindは、以下の循環を基本単位として動作する。

1. 自己を参照する（Self）
2. 記憶を参照する（Memory）
3. 行動を選択する（Decision）
4. 結果を通じて内部構造を更新する（Evolution）

### English
SeedMind operates on a recurring cycle:

1. Reference the self (Self)
2. Reference memory (Memory)
3. Select actions (Decision)
4. Update internal structure through outcomes (Evolution)

---

## Layered Structure

### 日本語
SeedMindのアーキテクチャは、概念的に以下のレイヤで捉えられる。

1. **Interface**  
   外部との接点。入力（知覚）と出力（発話・行動）を抽象化する。

2. **Interpretation**  
   入力を構造化し、内部で扱える形式へ変換する。判断は行わない。

3. **Self Model**  
   SeedMind自身の状態・制約・傾向・価値観を表現する参照モデル。

4. **Memory**  
   経験・知識・学習結果を保持し、将来の判断に影響を与える構造。

5. **Decision**  
   Self Model と Memory を参照し、行動・応答・沈黙を含む選択を行う中核。

6. **Expression**  
   選択結果を外部に伝達可能な形へ変換する（発話形式・応答形式など）。

7. **Action**  
   外部ツールやシステムと連携し、実際の行動を実行する。

8. **Reflection**  
   結果を観測・評価し、学習や更新に必要な情報を生成する。

9. **Evolution**  
   Reflectionの結果を用いて、Self Model・Memory・判断基準を更新する。

### English
Conceptually, SeedMind can be described in the following layers:

1. **Interface**  
   Boundary with the outside world. Abstracts inputs (perception) and outputs (speech/actions).

2. **Interpretation**  
   Structures inputs into internal representations. Does not decide.

3. **Self Model**  
   A reference model describing the current state, constraints, tendencies, and values of SeedMind.

4. **Memory**  
   A structure that stores experience/knowledge/learned results to influence future decisions.

5. **Decision**  
   The core that selects actions/responses/silence by referencing Self Model and Memory.

6. **Expression**  
   Converts selected intent into communicable outputs (e.g., response form, language).

7. **Action**  
   Executes real-world/tool/system actions.

8. **Reflection**  
   Observes and evaluates outcomes, producing signals for learning and updates.

9. **Evolution**  
   Updates Self Model, Memory, and decision criteria based on Reflection.

---

## Design Principles

### 日本語
- 判断は中核に集約される（Decision-centric）
- 記憶は保存ではなく、行動変化のために存在する
- 自己モデルは参照可能であり、説明可能である
- 最適化よりも一貫性と説明可能性を優先する
- レイヤは置き換え可能であり、固定実装を前提としない

### English
- Decision is centralized (decision-centric)
- Memory exists to change future behavior, not merely to store the past
- The self-model is referencable and explainable
- Consistency and explainability are prioritized over optimization
- Layers are replaceable; no single implementation is assumed

---

## Positioning

### 日本語
このOverviewは全体像を示すものであり、個別の手順や実装詳細を定義しない。  
具体的な動作手順は **Flow** を、構成要素の責務は **Components** を参照されたい。

### English
This overview presents the global structure and does not define step-by-step procedures or implementation details.  
For execution steps, see **Flow**. For responsibilities, see **Components**.
