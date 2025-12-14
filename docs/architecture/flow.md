# SeedMind Architecture — Flow

---

## 日本語

このドキュメントは、SeedMindにおける  
**1ターンの動作フロー**を定義する。

ここでいう「1ターン」とは、  
外部からの入力を受け取り、  
判断を行い、  
行動または応答を実行し、  
その結果を内部構造に反映するまでの一連の流れを指す。

このフローは単なる処理手順ではなく、  
SeedMindが「考え、選び、変化する存在」として振る舞うための  
最小単位である。

---

## English

This document defines a **single-turn execution flow** in SeedMind.

A “turn” refers to the sequence from receiving external input,  
through decision-making,  
to executing an action or response,  
and reflecting the outcome back into the internal structure.

This flow is not a procedural pipeline,  
but the minimal unit through which SeedMind behaves  
as an entity that thinks, chooses, and evolves.

---

## Overview of a Single Turn

### 日本語
1ターンは以下の段階で構成される。

1. Input（知覚）
2. Interpretation（解釈）
3. Self & Memory Reference（自己・記憶参照）
4. Decision（選択）
5. Expression / Action（表現・行動）
6. Reflection（評価）
7. Evolution（更新）

### English
A single turn consists of the following stages:

1. Input
2. Interpretation
3. Self & Memory Reference
4. Decision
5. Expression / Action
6. Reflection
7. Evolution

---

## Step-by-Step Flow

### 1. Input

#### 日本語
外部環境からの入力を受け取る段階。  
入力はテキスト、信号、状態変化など、形式を問わない。

この段階では、意味付けや判断は行わない。

#### English
The stage where input from the external environment is received.  
Inputs may be text, signals, or state changes.

No interpretation or decision is performed at this stage.

---

### 2. Interpretation

#### 日本語
入力を内部で扱える構造へ変換する段階。  
意味理解、文脈抽出、正規化などが行われる。

Interpretationは情報を整理する役割を持ち、  
行動の選択には関与しない。

#### English
Transforms input into a structure usable internally.  
Includes normalization, contextual extraction, and semantic structuring.

Interpretation organizes information but does not choose actions.

---

### 3. Self & Memory Reference

#### 日本語
解釈された情報をもとに、  
Self Model と Memory を参照する段階。

- 自身の状態・制約・傾向の確認  
- 過去の経験や知識の参照  
- 現在状況との整合性確認  

#### English
References the Self Model and Memory based on interpreted input.

- Check internal state, constraints, and tendencies  
- Recall past experiences and knowledge  
- Validate consistency with the current context  

---

### 4. Decision

#### 日本語
SeedMindの中核となる段階。  
Self Model と Memory を参照した上で、  
取るべき行動または応答を選択する。

沈黙や非介入も、意思決定の結果として扱われる。

#### English
The core stage of SeedMind.  
Selects actions or responses by referencing the Self Model and Memory.

Silence and non-intervention are also treated as valid decisions.

---

### 5. Expression / Action

#### 日本語
Decisionで選択された内容を、  
外部に実行可能な形へ変換・実行する段階。

- 発話として表現する  
- 外部ツールを操作する  
- 状態変化を引き起こす  

#### English
Converts and executes the selected decision in an external form.

- Express as speech  
- Operate external tools  
- Cause state changes  

---

### 6. Reflection

#### 日本語
行動または応答の結果を評価する段階。

- 結果の観測  
- 意図との乖離の検出  
- 内部モデルへの影響評価  

#### English
Evaluates the outcome of actions or responses.

- Observe results  
- Detect deviation from intent  
- Assess impact on internal models  

---

### 7. Evolution

#### 日本語
Reflectionの結果を用いて、  
内部構造を更新する段階。

- Memoryの更新  
- Self Model の調整  
- 判断基準の変化  

#### English
Updates internal structures based on reflection.

- Update memory  
- Adjust the self-model  
- Modify decision criteria  

---

## Characteristics

### 日本語
- フローはDecisionを中心に構成される  
- 各ターンは独立しているが、結果は蓄積される  
- 学習は外部処理ではなく、内部循環として発生する  

### English
- The flow is decision-centric  
- Each turn is independent, but outcomes accumulate  
- Learning occurs within the internal loop, not externally  

---

## Positioning

### 日本語
このFlowはSeedMindの動作原理を示すものであり、  
特定の実装や技術スタックを前提としない。

構成要素の責務については **Components** を参照されたい。

### English
This flow describes SeedMind’s operating principle  
without assuming any specific implementation or technology stack.

For component responsibilities, see **Components**.
