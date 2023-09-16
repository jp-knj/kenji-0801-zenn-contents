---
title: "ドキュメント戦略: チームの協力からツール選定まで"
---
## アクセシビリティをドキュメントにする理由
### アクセシビリティのためのドキュメント指針
デザインカンプやデザインドキュメントにアクセシビリティ情報を取り入れる手法は有効です。これにより、アクセシビリティに関する課題やシナリオを考えるための必要な筋肉を鍛えるのに役立ちます。

### アクセシビリティのプロセス
- すべてのデザインドキュメントにアクセシビリティ情報を追加すること。
- エンジニアへのデザインの引き渡しには、キーボードの動作、ラベル、意味論などの要素が含まれています。
- この取り組みは、製品のアクセシビリティを向上させるだけでなく、デザイナーがアクセシビリティを早い段階で考慮する能力を養うのにも役立ちます。
- アクセシビリティに関する議論を促進する。

プロダクトの初期段階では、アクセシビリティ設計のドキュメントは、キーボードの動作の定義と、支援技術が理解できるセマンティック・ラベルの指定が主になります。ドキュメントの複雑さを軽減し、より幅広いシナリオを考えるのに役立つからです。
色のコントラストやコンテンツのサイズ変更などの重要な要素は、デザインプロセスの初期段階で考慮することになると考えています。

### ドキュメントを執筆する担当者
- **PdM と PjM**: アクセシビリティを初期段階で考慮して、プロダクトのアクセシビリティ要件を定義し、チームとしてシームレス、スマートに取り組めるようにドキュメントにまとめる
- **デザイナー**: カラー、タイポグラフィのような要素のコントラストや予測可能なレイアウトで構造化して、デザインの詳細や動作をドキュメントする
- **開発者とアクセシビリティ専門家**: 複雑なアクションの代替やキーボード操作可能にして、支援技術が解釈可能なセマンティック・ラベルの指定するなどの技術的な詳細と実装をドキュメントする
- **コンテンツ、UXライター、SEO担当者**: コンテンツ、代替テキスト、SEO に関する情報をドキュメントする
- **テスターとQA**: アクセシビリティに関するテストケースを作成する

### 効果的なドキュメントの執筆方法
- **ユーザーのフィードバックを取り入れる**: ドキュメントの作成前にユーザーとの対話を通じて情報収集する。
- **簡単なツールから始める**: ドキュメントの障壁を下げるために、使い慣れたツールでの記述を始める。
- **継続的な更新**: 常に最新の情報を反映させるため、定期的にドキュメントを見直し・更新する。

### ドキュメント作成のタイミング
技術的な実現可能性を確認し、最終的なコンポーネントやページの完成後にドキュメントにまとめる。

## チームの協力とアクセシビリティの促進
### イントロダクション:
プロセス、構造、生産性、貢献、接続の理解は簡単に見えるように思えますが、その状態に達するまでの道のりは容易ではありません。実際のコラボレーションは、時間、努力、そしてケアを組み合わせて継続的に向上を追求するプロセスです。

### チーム構築における主要な疑問
- 自発的なコラボレーションは難しい。効果的な協力のための継続的な探求が求められます。
- 最適なワークフローを見つけるための主要な疑問：
    - 最適なチームモデルは
    - チームリーダーは誰か
    - どのように意思決定を行うか

#### チームセットアップのヒント
- チームサイズよりも、各部署を繋げ、シロ化を避けることに重点を置く。
- リソースや予算が制限されている場合、最も価値をもたらすセットアップを求める。

#### チームモデルの種類
- 分離型： デザインシステムチームが単独で製品の最善を追求。しかし、柔軟性に欠けます。
    - デザインシステムチームは、自分たちがプロダクトに基づいてデザインシステムを構築します。彼らは人々にデザインシステムから情報を引き出させようとします。チームとして、同盟関係も日々の活動も見ることができず、"取るか取られるか "という感じです。これが何を意味するかは誰もが知っています。
- 中心型： 組織の中心で動くが、各製品チームとの連携が必要です。
    - デザインシステムチームが組織の中心に位置し、プロダクトチームにサービスを提供します。このモデルには、日常的なコラボレーションや、プロダクトチームの優先順位の確認が必要です。そのため、各チームは新しいシナリオに基づいてコンポーネントの適合を開始し、更新されたコンポーネントのシステムへの実装を見ます。
- 浸透型： 中心型と"大使"の組み合わせ。プロダクトの各チームに"大使"が存在し、デザインシステムチームと継続的に連携。私が "immersed "と名付けたのは、集中型モデルと各プロダクトチームの "アンバサダー "を組み合わせになります。アンバサダーはコアとなる貢献者であり、デザインシステムのミーティングに出向き、新機能について学び、チームに説明します。このモデルは、エンジニア、デザイナー、チームリーダーなどをつなぐ、コミュニティ主導の取り組みです。彼らのインプットがデザインシステムの価値を高めるのに役立つため、より高い品質が保証されます。このモデルでは、プロダクトに関わるすべての人がフィードバックを得たり与えたりできるため、デザインシステムチームは構造全体の重要な一部となります。

#### 貢献とコミュニケーション
貢献は即座に理解可能でなければならず、同僚を物語の一部として参加させることが必要です。接続と受け入れのための共有の所有権を作成します。

**コミュニケーションツール:**
- Slack, Discord
- 定期的なオフィス時間
- 週次/隔週の通話
- 内部ニュースレター
- 教育的なガイドやビデオ

#### カスタムデザインシステムの構築
Figma の API を利用してデザインをテックスタックに統合。
他のオプションとして Sketch API や Vercel、Netlify があります。

---
## ドキュメンテーションツールの選択ガイド
### ゼロから始める
デザインシステムが初めてで 1 年目の場合は既存の解決策に頼りましょう。Zeroheight、Supernova、Knapsack、Specify、Backlight のような既存のツールを選択することをお勧めします。この段階では、命名規則やシステムの構築など、ミスがよくあります。これらのツールを使用することで、基本的な部分に集中できます。

#### 既存のデザインシステムをアップグレード
既に確立されたデザインシステムを持つ大手企業の場合、全体的な改善は必要ありません。まず、現在のシステムの強みと弱みを評価してからアップデートしてください。

#### 法的およびセキュリティ基準を遵守
銀行のように厳格なセキュリティ要件を持つ業界では、サードパーティのアプリを介しての共有は限られています。ここでは、カスタムビルドのために Figma API を利用するのが最も適している可能性があります。

### ドキュメンテーションツールの概要
#### 基本的なツール
- **Airtable:** デザインシステムがまだ完全に開発されていない場合に最適。さまざまなプラットフォームのデザインコンポーネントをリストアップするための動的なテーブルを作成できます。
- **Notion:** 基本的なデザインシステムバージョンに適しています。Figma や Storybook との統合はスムーズではありませんが、基本的なコンポーネントの説明には役立ちます。
- **GitHub Pages:** GitHub リポジトリから直接ホストできます。GitHub の使用に慣れる必要がありますが、リアルタイムの更新には効果的です。

#### 既製のソリューション
- **Zeroheight:** クロスファンクションのチームに理想的で、デザインドキュメンテーションを開始するためのテンプレートを提供しています。
- **Supernova:** デザイントークンに重点を置いている新しいツールです。ノーコード機能と組み込みのコードエディタを提供しています。
- **Knapsack:** コードとデザインを統合するプラットフォームで、開発者とデザイナーがリアルタイムで協力して作業できます。
- **Specify:** 基本的にはデザイン API で、デザインツールを中心化します。自動更新をサポートし、Figma や GitHub とシームレスに統合されています。

#### 高度なソリューション
- **Storybook:** UI コンポーネントの作成とテストのためのツール。ガイドラインをより包括的にするために、他のツールとの統合が必要となる場合があります。

### 総括
1 つの解決策がすべてに適しているわけではありません。選択は、チームの独自のニーズとデザインシステムが広く採用されることを助けるものとして合致するべきです。

https://www.kotobaux.com/blog/6-steps-to-creating-a-ux-writing-style-guide