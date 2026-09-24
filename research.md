---
layout: default
title: 研究
permalink: /research/
eyebrow: Research
description: 五島研究室の研究テーマ、教員の論文、学生の研究成果を紹介します。
---

五島研究室では、ファイナンス（Finance）とデータサイエンス（Data Science）を組み合わせた実証研究を行っています。計量経済学・統計学の手法に加えて、自然言語処理や機械学習などの計算機科学の手法を用い、株価・取引データ・企業情報・ニュース記事などのデータを分析しています。

以下では主な研究テーマと、それぞれに関連する教員の論文を紹介します。学生の研究テーマはこれらに限らず、各自の関心に基づいて設定します。

<nav class="jump" aria-label="ページ内リンク">
  <a href="#text">テキストデータと金融市場</a>
  <a href="#ml">機械学習の金融応用</a>
  <a href="#market">市場の構造とリスク</a>
  <a href="#climate">気候変動・ESGとファイナンス</a>
  <a href="#students">学生の研究成果</a>
</nav>

<section class="theme-block" id="text">
  <h2><span class="en">Text Data</span>テキストデータと金融市場</h2>
  <p>ニュース記事や有価証券報告書などのテキストを自然言語処理で数値化し、市場や経済の状態を表す指標をつくる研究です。これまでに、株価の情報を用いた金融分野の極性辞書や景気単語の極性辞書の構築、ニュースから作成した景況感指数によるボラティリティやインフレの予測、有価証券報告書における経営者の将来見通しの開示と業績の関係の分析などに取り組んできました。</p>
  <details class="papers-toggle"><summary>関連する論文</summary>{% include papers.html tag="text" %}</details>
</section>

<section class="theme-block" id="ml">
  <h2><span class="en">Machine Learning</span>機械学習の金融応用</h2>
  <p>深層学習をはじめとする機械学習の手法を、金融データの分析に応用する研究です。ニュース記事の評判分析、株価の時系列データから市況コメントを自動生成する研究（自然言語生成）、因果推論のための機械学習（Double Machine Learning）を用いた分析などに取り組んできました。科研費の研究課題として、ファイナンスデータに対する説明可能な機械学習手法の開発にも取り組みました。</p>
  <details class="papers-toggle"><summary>関連する論文</summary>{% include papers.html tag="ml" %}</details>
</section>

<section class="theme-block" id="market">
  <h2><span class="en">Market &amp; Risk</span>市場の構造とリスク</h2>
  <p>金融市場の構造や、市場で生じるリスクを実証的に分析する研究です。国際株式市場間の連動性の長期的な変化、暗号資産市場のメルトダウンリスク、金融政策の発表と外国為替市場におけるアルゴリズム取引の関係、高頻度取引（HFT）と他の投資家の相互作用などを扱ってきました。</p>
  <details class="papers-toggle"><summary>関連する論文</summary>{% include papers.html tag="market" %}</details>
</section>

<section class="theme-block" id="climate">
  <h2><span class="en">Climate &amp; ESG</span>気候変動・ESGとファイナンス</h2>
  <p>気候変動や企業の環境・社会への取り組みが、金融市場や企業のパフォーマンスとどのように関係するかを分析する研究です。東京株式市場におけるカーボンプレミアム、CO2排出量と企業パフォーマンスの関係、CSR活動に関するニュースが株価に与える影響などを分析してきました。現在は、科研費の研究課題「金融市場における気候変動リスク計測に関する研究」（2024–2026年度）に取り組んでいます。</p>
  <details class="papers-toggle"><summary>関連する論文</summary>{% include papers.html tag="climate" %}</details>
</section>

<section class="band" id="students">
  <h2><span class="en">Student Research</span>学生の研究成果</h2>
  <p>研究室に所属する学生の学会・コンペティションでの発表です。</p>
  {% include student-pubs.html %}
</section>

<h2><span class="en">Faculty Publications</span>教員の論文一覧</h2>

教員の論文の一覧は[教員紹介]({{ '/teacher/' | relative_url }}#papers)に掲載しています。講演などを含む業績の全体は[researchmap]({{ site.researchmap }})をご覧ください。
