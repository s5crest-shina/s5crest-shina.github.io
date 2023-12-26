---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: markdown
    design:
      columns: '1'
      background:
        gradient_start: 'navy'
        gradient_end: '#a44'
        gradient_angle: 180
        text_color_light: true
    content:
      text: |
        <div class="title">
        <a href="https://www.jst.go.jp/kisoken/crest/index.html">JST CREST （戦略的創造研究推進事業）</a><br>
        <a href="https://www.jst.go.jp/kisoken/crest/research_area/ongoing/bunya2021-2.html">基礎理論とシステム基盤技術の融合によるSociety 5.0のための基盤ソフトウェアの創出 （S5基盤ソフト）</a><br>
        2022年度採択課題
        <h1>隔離実行と形式検証による総合的セキュリティ基盤システム</h1>
        <h2>研究代表者: 品川 高廣 （東京大学）</h2>
        </div>

  - block: markdown
    id: overview
    design:
      columns: '2'
    content:
      title: 研究概要
      subtitle:
      text: |
        {{< figure src="overview.png" caption="FrieOS Project" width="100%" numbered="true" >}}
        Society 5.0をサポートするために、システム全体に強固なセキュリティを提供する包括的なセキュリティ基盤としてのオペレーティングシステムを実現する。

        最先端のハードウェア技術やシステムソフトウェア技術によって実現される隔離実行環境を、セキュリティにフォーカスした形式手法によって効率的に強化することで、理論的に検証されたセキュリティの実用システムへの適用を容易にする。

        また、プログラミング言語理論のサポートにより、エッジ（末端）からクラウド（中心）まで包括的なセキュリティポリシーを適用することで、システム全体の一貫したセキュリティを実現する。

  - block: people
    id: people
    design:
      columns: '2'
    content:
      title: 研究体制
      user_groups:
          - 品川グループ
          - 住井グループ
          - 広渕グループ
      sort_by: Params.order
      sort_ascending: true
    design:
      show_interests: false
      show_role: false
      show_organizations: true
      show_social: false

  - block: collection
    id: papers
    content:
      title: 論文
      filters:
        folders:
          - publication
    design:
      columns: '2'
      # Choose your content listing view - here we use the `showcase` view
      view: citation
      # For the Showcase view, do you want to flip alternate rows?
      # flip_alt_rows: true
---
