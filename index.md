---
layout: default
title: ホーム
permalink: /
eyebrow: Finance × Data Science
hero: '<span>金融市場を、</span><span>データで読み解く。</span>'
hero_lead: 横浜国立大学・五島研究室では、ファイナンスとデータサイエンスを掛け合わせ、株価・企業情報・ニュースなどのデータから金融市場の仕組みを明らかにする研究に取り組んでいます。
hero_buttons:
  - label: 学部ゼミを見る
    url: /seminar/
    style: white
  - label: 大学院を見る
    url: /graduate/
    style: ghost
has_contact: true
---

<h2 class="center"><span class="en">For Students</span>あなたに合った入口から</h2>

<div class="paths">
  <a class="path path-light" href="{{ '/seminar/' | relative_url }}">
    <span class="path-label">経営学部の学部生へ</span>
    <h3>未経験から、<br>学会発表まで。</h3>
    <p>データ分析と投資理論を、仲間と一緒にゼロから学ぶゼミです。</p>
    <ul>
      <li>プログラミング経験は選考に関係なし</li>
      <li>3年次はチームでコンペに挑戦</li>
      <li>学会やコンペで成果を発表</li>
      <li>合宿なし。就活・留学とも両立</li>
    </ul>
    <span class="path-more">学部ゼミについて {% include icon.html name="arrow" %}</span>
  </a>
  <a class="path path-navy" href="{{ '/graduate/' | relative_url }}">
    <span class="path-label">大学院進学を考えている方へ</span>
    <h3>研究者として、<br>本格的に鍛える。</h3>
    <p>学会発表と査読付き論文の掲載を目標に、実証研究に取り組みます。</p>
    <ul>
      <li>週1回のミーティングで継続指導</li>
      <li>学会発表・論文投稿まで伴走</li>
      <li>研究経費は研究室予算で可能な限り負担</li>
      <li>コアタイムなし。社会人も歓迎</li>
    </ul>
    <span class="path-more">大学院について {% include icon.html name="arrow" %}</span>
  </a>
</div>

<section class="band">
  <h2><span class="en">Research</span>研究テーマ</h2>
  <p>計量経済学や統計学に加えて、自然言語処理・機械学習・深層学習などの計算機科学の手法を組み合わせ、ファイナンスデータの実証研究を行っています。</p>
  <div class="features">
    <div class="feature">
      <span class="feature-icon">{% include icon.html name="chart" %}</span>
      <h3>計量ファイナンス</h3>
      <p>株式市場データや資産価格データを用いて、投資リスクの定量分析、資産価格の予測モデル開発、市場アノマリーの検証などに取り組みます。</p>
    </div>
    <div class="feature">
      <span class="feature-icon">{% include icon.html name="text" %}</span>
      <h3>テキストデータ分析</h3>
      <p>ニュース記事や企業開示資料、SNSなどのテキストを自然言語処理で解析し、金融市場との関係を実証的に分析します。</p>
    </div>
    <div class="feature">
      <span class="feature-icon">{% include icon.html name="ai" %}</span>
      <h3>機械学習・AIの金融応用</h3>
      <p>機械学習や深層学習をファイナンスに応用し、資産価格の予測や説明可能なAI、気候変動リスクの計測などに取り組みます。</p>
    </div>
  </div>
</section>

<h2><span class="en">Lab at a Glance</span>数字で見る五島研究室</h2>

<div class="stats">
  <div class="stat"><span class="stat-num">10<small>名</small></span><span class="stat-label">学部ゼミ生（2026年・3〜4年生）</span></div>
  <div class="stat"><span class="stat-num">0<small>時間</small></span><span class="stat-label">コアタイム</span></div>
  <div class="stat"><span class="stat-num">約1<small>名</small></span><span class="stat-label">大学院へ進学（例年・各学年）</span></div>
  <div class="stat"><span class="stat-num">約1<small>名</small></span><span class="stat-label">留学（例年・各学年）</span></div>
</div>

<h2><span class="en">News</span>お知らせ</h2>

<ul class="news-list">
{% for n in site.data.news %}
  <li><span class="news-date">{{ n.date }}</span><span>{% if n.link %}<a href="{{ n.link | relative_url }}">{{ n.text }}</a>{% else %}{{ n.text }}{% endif %}</span></li>
{% endfor %}
</ul>

{% include contact.html text="ゼミや大学院進学についての相談、共同研究・取材・講演のご依頼など、お気軽にご連絡ください。" %}
