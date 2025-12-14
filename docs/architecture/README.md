# SeedMind Architecture

---

## 日本語

このディレクトリは、SeedMindのアーキテクチャを定義するためのドキュメント群を収録している。

ここで扱うアーキテクチャは、実装構成を示すものではなく、  
SeedMindの思想を具体的な構造として成立させるための設計である。

SeedMindの中核には、  
自己を参照し（Self）、  
記憶を参照し（Memory）、  
行動を選択し（Decision）、  
その結果を通じて構造自体を更新していく（Evolution）  
という循環がある。

本ディレクトリのドキュメントは、  
この循環をどのような構造として表現するかを示す。

---

## English

This directory contains documents that define the architecture of SeedMind.

The architecture described here is not an implementation layout,  
but a structural representation of the SeedMind conceptual framework.

At the core of SeedMind lies a continuous cycle:  
referencing the self (Self),  
referencing memory (Memory),  
selecting actions (Decision),  
and updating the structure itself through outcomes (Evolution).

These documents describe how this cycle is realized as an architectural structure.

---

## Documents

### 日本語

- **overview.md**  
  SeedMindの全体構造と、各レイヤの責務を説明する。

- **flow.md**  
  入力から判断、行動、振り返りまでの  
  1ターンの動作フローを定義する。

- **components.md**  
  アーキテクチャを構成する主要コンポーネントの  
  責務と役割を定義する。

### English

- **overview.md**  
  Describes the overall structure of SeedMind and the responsibility of each layer.

- **flow.md**  
  Defines a single-turn execution flow from input to action and reflection.

- **components.md**  
  Defines the responsibilities of the core components that constitute the architecture.
  
