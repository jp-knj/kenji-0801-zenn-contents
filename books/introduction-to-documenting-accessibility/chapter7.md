---
title: "[WIP] インタラクションを支えるポイントジェスチャー"
---
## ポイントジェスチャーについて

ポインタージェスチャーとは、支援技術を用いて、人が機能的なコントロールを操作するために行う動作のこと
- 指
- マウス
- ヘッドポインター
- 視線システム

一部のポインタージェスチャーは、特定の人にとって実行が困難であったり、不可能であったりする場合があるため、アクセシブルな代替手段が必要となる場合があります。

### ポインター・ジェスチャーとアクセシビリティ
今日のユーザーインターフェースの多くは、ポインティングやクリック以外のジェスチャーを必要とします。

- メディアプレーヤーのオーディオボリュームを変更するには、トグルをスライダーの上下に動かす必要があるかもしれない。
- ToDoアプリでタスクを整理するには、ページのある領域から別の領域に項目をドラッグする必要があるかもしれません。

タッチスクリーン・デバイスの普及は、キーボードやマウスだけでは不可能だった操作を、指を使って行う新しいジェスチャーを多くの人が学ばなければならなくなったことも意味している。

人によっては、これらのジェスチャーを正確に行うことが難しかったり、ジェスチャーがまったくできなかったりすることがあります。

具体例を挙げると
手先が不器用な人や手の震えがある人は、あるジェスチャーを正確に行うことが難しい場合があります。
 - スワイプ
 - ドラッグ
 - ピンチ 
ヘッドワンドを使用している人は、比較的簡単なジェスチャーしかできないかもしれません。認知障害や学習障害のある人は、理論的には必要なジェスチャーを行うことができても、その方法を理解していない場合がある。

### ポインタージェスチャーを理解する
ポインタージェスチャーには、主に以下の4種類があります：
- シングルポインタージェスチャー
- マルチポイントジェスチャー
- パスベースのジェスチャー
- ドラッグ動作

コンフォーマンスの観点から、ウェブコンテンツ・アクセシビリティ・ガイドラインは、ドラッグ動作と他のポインタ・ジェスチャーを明確に区別していることに注意してください。

マルチポイントジェスチャーとパスベースのジェスチャーは WCAG 2.1 で導入された 2.5.1 Pointer Gestures (Level A)でカバーされ、ドラッグ動作は WCAG 2.2 で導入された 2.5.7 Dragging Movements (Level AA) で個別にカバーされます。

https://www.w3.org/TR/WCAG21/#pointer-gestures

https://www.w3.org/TR/WCAG22/#dragging-movements

### シングルポインタージェスチャー
シングルポインター・ジェスチャーは、マウスやタッチスクリーン上の 1 本の指／スタイラスを使うだけで、最も簡単に実行できます。

シングルポインタージェスチャーの代表的な例には、以下のようなものがあります：
- クリック：ダブルクリックを含む
- タップ：ダブルタップを含む
- プレス：プレス＆ホールドを含む
- スワイプ: コントロールの操作にスワイプの角度が関係ない場合（以下のパスベースのジェスチャに関する注記で詳しく説明します）

ボタン、リンク、チェックボックスは通常、シングルポインタ・ジェスチャーのみで簡潔します。

### マルチポイント・ジェスチャー
マルチポイント・ジェスチャーとは、複数のポインターを同時に使うジェスチャーです。このようなジェスチャはタッチスクリーン環境では一般的です。

マルチポイント・ジェスチャーの代表的な例には、以下のようなものがあります：

- 2本の指をピンチする／広げる：地図アプリケーション内でのピンチ・トゥ・ズームを含む。
- 2本指での回転：ダイヤルコントロールを操作するための2本指での回転など。
- 複数の指を使ったタップ：リスト内の複数項目の選択など

### アクセシブルな代替機能の作成
特定のジェスチャを行うことが困難または不可能な障害者をサポートするために、関連する WCAG 成功基準では、操作に
- マルチポイントジェスチャ
- パスベースのジェスチャ、
- ドラッグ動作

を使用するすべての機能は、パスベースではない単一のポインタジェスチャを使用しても操作可能でなければならないと述べています。

例外は以下の通り：
- ジェスチャが必須であること。
    - 例えば、ステディハンドゲームは、人が細かい運動を含むジェスチャを使用できることに依存しています。
      機能がユーザーエージェントによって決定され、作者によって変更されない。
- デバイスに内蔵されたスクリーンリーダーによって提供される機能などである。

実際には、通常同じ機能を実行する別のコントロールをデザインに追加しますが、シングルタップやシングルクリックのような単一のポインタジェスチャしか必要としません。

パスベースのジェスチャーに関する注意
上述したように、パスベースのジェスチャーを必要とするすべての機能に対して、パスベースではない単一のポインターベースの代替手段を提供する必要があります。

しかし場合によっては、ジェスチャがパスベースであるかどうか、したがってそのような代替手段が必要かどうかを解釈することが、混乱を招くことがあります。これは、ジェスチャーを行う際に人がたどるべき経路が明示的または明白に存在しない場合に典型的です。

つまり、ジェスチャーの正確さです。つまり、ジェスチャーの正確さである：

ジェスチャーの角度や方向が成功に影響しない場合、そのジェスチャーはパスベースのジェスチャーではなく、代替案は必要ありません。

ジェスチャの角度や方向が成功に影響する場合、そのジェスチャはパスベースであり、パスベースではない単一のポインタベースの代替手段が必要です。
これは例で説明するのが一番わかりやすいでしょう。

次のスクリーンショットは、典型的なカルーセルを示しています。人が画面を左右にスワイプしてスライドを移動させます。スワイプジェスチャーの角度や方向は、カルーセルが動くかどうかに影響しない。たとえジェスチャーが少し斜めに行われたとしても、カルーセルは人がスクリーンを横切ってまっすぐスワイプした場合と同じように動作する。したがって、2.5.1 ポインタ・ジェスチャー（レベルA）を満たすために、単一のポインタ・ベース、非パス・ベースの代替手段は必要ない。

ただし、カルーセルがドラッグ操作にも依存している場合は、代替手段の欠如が2.5.7 ドラッグ操作（レベルAA）の不合格の原因となる可能性があることに注意すること。

https://www.w3.org/TR/WCAG21/#pointer-gestures

https://www.w3.org/TR/WCAG22/#dragging-movements

次のスクリーンショットは、同じカルーセルを示しています。ただし今回は、スワイプの角度が左から右、または右から左に完全にまっすぐでなければなりません。例えば、人が少し斜めにスワイプするなど、ずれがあると、カルーセルは期待通りに動きません。そのため、このような場合は、パスベースではない、単一のポインターベースの代替手段が必要となります。

スワイプを成功させるために特定の経路をたどる必要がある場合、単一ポインタ、非経路ベースの代替手段が必要となる。とはいえ、ジェスチャーの角度や方向、精度がジェスチャーの成功に影響しない場合でも、すべてのケースでシングルポインター、パスベースでない代替手段を提供することはグッドプラクティスです。そうすることで、ジェスチャーがパスベースでない場合でも、すべての人、特にジェスチャーが難しいと感じる人にメリットがあります。さらに、コンポーネントの操作に何らかのドラッグ動作が必要な場合は、代替手段が必要であることを覚えておいてください。