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
        <a href="https://www.jst.go.jp/kisoken/crest/en/index.html">JST CREST (Strategic Basic Research Programs)</a><br>
        <a href="https://www.jst.go.jp/kisoken/crest/en/research_area/ongoing/area2021-2.html">Creation of System Software for Society 5.0 by Integrating Fundamental Theories and System Platform Technologies<br>(Society 5.0 System Software)</a><br>
        Year Started : 2022
        <h1>A Comprehensive Security Infrastructure System with Isolated Execution and Formal Verification</h1>
        <h2>Research Director: Takahiro Shinagawa (The University of Tokyo)</h2>
        </div>

  - block: markdown
    id: overview
    design:
      columns: '2'
    content:
      title: Research Overview
      subtitle:
      text: |
        {{< figure src="overview.en.png" caption="FormarieOS Project" width="100%" numbered="true" >}}
        In order to support Society 5.0, we realize an operating system that serves as a comprehensive security infrastructure to provide strong security throughout the system.

        We facilitate the application of theoretically verified security to practical systems by efficiently reinforcing isolation execution environments enabled by state-of-the-art hardware and system software technologies with the support of security-focused formal methods.

        We also ensure consistent security throughout the system by enforcing comprehensive security policies from the edge (end) to the cloud (center) with the support of programming language theory.

  - block: people
    id: people
    design:
      columns: '2'
    content:
      title: Research Organization
      user_groups:
          - Shinagawa Group
          - Sumii Group
          - Hirofuchi Group
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
      title: Publication
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
