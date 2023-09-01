---
title: "[WIP] インタラクションのドキュメントについて"
---
## インタラクションの文書化
### インタラクションの状態とステータス
インタラクティブなコンポーネントに対して、私が最初に文書化しようとするのは、異なるステートです。

私の例では、さまざまなボタンの状態を文書化している：
- デフォルト
- ホバー
- フォーカス
- アクティブ

フォーカスの状態はアクセシビリティにとって重要です。

キーボード・ユーザーがページをナビゲートするときに、自分がどこにいるのかを知るのに役立ちます。
また、"loading "のような「HTML公式ではない」状態を追加することもできます。

チェックボックスには

- default
- focus
- checked
- disabled、
- disabled checked、
- indeterminate
- disabled indeterminate。

最後の2つはHTMLの仕様にはありません。

しかし、ユーザーが複数の行をチェックできるようなテーブルでは、時々必要になります。ラジオボタンも同じですが、indeterminate でないことを除きます。

フォームの input については、コンポーネント・レベルで、
- default
- focus
- filled
- disabled (read only)

という一般的な分類があります。

しかし、例えば、いくつかの追加ステータスを持つことができます：

- error
- success
- information

色だけでなく、テキストやアイコンも使用するでしょう（色だけが情報を伝える方法ではない）。

コンポーネントが使用されるページレベルでは、より明確に指定する必要があります。
右は、フィルターで使用される年入力の例です。 文書化：
- 何がエラーを引き起こすのか（＝エラーケース）
- 正確なメッセージ（コピー）はどうあるべきか。

## マウスとキーボード入力を文書化するインタラクション・フロー
多くのインタラクションを持つ複雑なコンポーネントのために、私は「インタラクション・フロー」を構築。

さまざまなインタラクションがある場合、これらのコンポーネントがどのように動作すべきかをドキュメントに残しましょう。


チェックボックス付きのフィルターを持っています。ユーザがチェックボックスにチェックを入れるとどうなるかを、順を追って説明：

- フィルタを開く、
- 要素にカーソルを合わせる
- フィルターボックスをチェックする、
- 適用ボタンを押す

マウスのインタラクションに加えて、キーボードのインタラクションも記録。
このコンポーネントでもキーボードナビゲーションを表示する、同様のフローに行き着きます：

- コンポーネントを開く方法（enter/space）、閉じる方法（esc）
- 要素間を移動する方法（上下キー）
- ボックスをチェックする方法

https://www.washington.edu/accesstech/checklist/keyboard/

https://tetralogical.com/blog/2021/10/26/browsing-with-a-keyboard/

https://webaim.org/techniques/keyboard/#testing

**キーボード・ナビゲーションを文書化する際に役立つ、ちょっとした備忘録**

- Tabキーでセクション間をジャンプ
- 矢印キーは、コンポーネント内を移動するのに役立ちます
- スペース/エンターキーは、要素をアクティブにします。

**あいまいなリンク**
- 要素の "クリック可能 "な部分がはっきりしないことがあります。特に、コンポーネント全体を包んでいる場合。

**複雑なジェスチャーの代替**
- アクセシビリティとユーザビリティのベストプラクティス。例として、gmailの「右スワイプ」によるアーカイブ機能が挙げられます。

gmail の代替案を文書化するとしたら、次のようなことができるだろう。
複雑なジェスチャーを、右にスワイプしてアーカイブすることを示すモックアップとともに文書化

それから代替案を文書化する：
- メールを長押ししてツールバーを表示し、アーカイブアイコンを押す。
- メールを開き、上部のアイコンを押す。
- 何が複雑なジェスチャーなのか、あるいはそうでないのか

https://tetralogical.com/blog/2023/03/17/foundations-pointer-gestures/

### ズームの動作
複雑なレスポンシブ・ページの場合、「ズーム」の動作を文書化することもできます。ユーザーは、コンテンツを壊すことなく、サイトを400％まで拡大できるようにする必要があります（隠しテキストや画像などはありません）。

私は開発チームに、ズームの動作（と高さ）をブロックしないようにお願いしています。そして、さまざまな解像度やブラウザのズームレベルでサイトをテストしています。

文書化するのがかなり厄介なデザインの側面の1つに、アニメーションとトランジションがある。これらにもアクセシビリティのベストプラクティスがあります。アニメーションやトランジションの中には、乗り物酔いを引き起こすユーザーもいる。ちなみに私もその一人だ。

`prefers-reduced-motion` メディアクエリを使えば、動きの少ないものを好む人のために代替バージョンを提供することができます。

https://stephaniewalter.design/blog/enhancing-user-experience-with-css-animations/#accessibility