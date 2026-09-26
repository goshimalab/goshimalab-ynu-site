---
layout: default
title: ホーム
permalink: /
eyebrow: Finance × Data Science
hero: '<span>金融市場を、</span><span>データで読み解く。</span>'
hero_lead: 横浜国立大学 五島研究室は、ファイナンスとデータサイエンスを組み合わせた実証研究を行う研究室です。
has_contact: true
---

<h2><span class="en">About</span>研究室について</h2>

横浜国立大学・五島研究室では、ファイナンス（Finance）×データサイエンス（Data Science）をテーマとした研究活動に取り組んでいます。計量経済学や統計学に基づく手法に加えて、自然言語処理や機械学習、深層学習などの計算機科学の手法を組み合わせ、ファイナンスデータを対象とした実証研究を行っています。

経営学部での学部ゼミと、大学院（国際社会科学府・先進実践学環）での研究指導を行っています。

<h2><span class="en">What You Learn</span>学べること</h2>

<div class="features">
  <a class="feature feature-link" href="{{ '/seminar/#finance' | relative_url }}">
    <span class="feature-icon">{% include icon.html name="chart" %}</span>
    <h3>ファイナンス</h3>
    <p>投資のリスク、資産価格の予測、経済と金融市場の関係など、金融市場のしくみを実際のデータを使って学びます。</p>
  </a>
  <a class="feature feature-link" href="{{ '/seminar/#datascience' | relative_url }}">
    <span class="feature-icon">{% include icon.html name="ai" %}</span>
    <h3>データサイエンス</h3>
    <p>統計学、計量経済学、機械学習、自然言語処理を学び、Python で自分で分析できるようにします。</p>
  </a>
  <a class="feature feature-link" href="{{ '/seminar/#research' | relative_url }}">
    <span class="feature-icon">{% include icon.html name="paper" %}</span>
    <h3>研究の進め方</h3>
    <p>論文を読み、問いを立て、データで検証し、論文にまとめて学外で発表するまでを経験します。</p>
  </a>
</div>

<p>詳しくは<a href="{{ '/seminar/' | relative_url }}">学部ゼミ</a>・<a href="{{ '/graduate/' | relative_url }}">大学院</a>のページをご覧ください。</p>

<section class="band">
  <h2><span class="en">For Students</span>学生の方へ</h2>
  <p>五島研究室では、「ファイナンス×データサイエンス」を中心とした研究に意欲的に取り組みたい学生を歓迎します。学部ゼミ・大学院とも、ファイナンスやデータ分析に関心のある方の応募をお待ちしています。</p>
  <div class="paths">
    <a class="path path-light" href="{{ '/seminar/' | relative_url }}">
      <span class="path-label">経営学部の学部生</span>
      <h3>学部ゼミ</h3>
      <p>投資理論とデータサイエンスを学ぶゼミです。2・3年次に輪読や演習、グループでのコンペティション参加を通じて基礎を身につけ、4年次に卒業論文に取り組みます。</p>
      <ul>
        <li>プログラミングやデータ分析の初学者も歓迎します（選考は面接のみ）</li>
        <li>学会やデータ分析コンペでの発表を目標とします</li>
      </ul>
      <span class="path-more">学部ゼミの案内 {% include icon.html name="arrow" %}</span>
    </a>
    <a class="path path-navy" href="{{ '/graduate/' | relative_url }}">
      <span class="path-label">大学院進学を検討している方</span>
      <h3>大学院（修士・博士）</h3>
      <p>週1回のミーティングを軸に研究を進め、学会発表と査読付学術雑誌への投稿を目指します。学内・学外、文系・理系を問わず歓迎します。</p>
      <ul>
        <li>入学前の面談が可能です（オンライン可）</li>
        <li>修士課程は、筆記試験のない内部進学試験・推薦入学試験・特別選抜で進学できます</li>
      </ul>
      <span class="path-more">大学院の案内 {% include icon.html name="arrow" %}</span>
    </a>
  </div>
  <p>For prospective international students: <a href="{{ '/en/graduate/' | relative_url }}">Graduate School (English)</a></p>
</section>

<h2><span class="en">News</span>お知らせ</h2>

<ul class="news-list">
{% for n in site.data.news %}
  <li><span class="news-date">{{ n.date }}</span><span>{% if n.link %}<a href="{{ n.link | relative_url }}">{{ n.text }}</a>{% else %}{{ n.text }}{% endif %}</span></li>
{% endfor %}
</ul>

<h2><span class="en">Overview</span>研究室の概要</h2>

<div class="table-wrap">
<table class="compare info">
  <tbody>
    <tr><th>名称</th><td>横浜国立大学 五島研究室</td></tr>
    <tr><th>教員</th><td><a href="{{ '/teacher/' | relative_url }}">五島 圭一</a>（大学院国際社会科学研究院 准教授）</td></tr>
    <tr><th>学部</th><td>経営学部（学部ゼミ）</td></tr>
    <tr><th>大学院</th><td>国際社会科学府（修士課程・博士後期課程）、先進実践学環（修士課程）</td></tr>
    <tr><th>研究分野</th><td>ファイナンス、データサイエンス、自然言語処理、機械学習</td></tr>
    <tr><th>学部ゼミ生</th><td>4年生 7名、3年生 3名（2026年）</td></tr>
  </tbody>
</table>
</div>

{% include contact.html text="共同研究・取材・講演のご相談や、ゼミ・大学院進学に関するご質問は、下記のメールアドレスまでご連絡ください。" %}
