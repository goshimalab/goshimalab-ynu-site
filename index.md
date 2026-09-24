---
layout: default
title: ホーム
hero: 金融市場を、データで読み解く。
permalink: /
---

## 研究室紹介

<p class="lead">横浜国立大学・五島研究室では、ファイナンス（Finance）×データサイエンス（Data Science）をテーマとした研究活動に取り組んでいます。計量経済学や統計学に基づく手法に加えて、自然言語処理や機械学習、深層学習などの計算機科学手法を組み合わせることで、ファイナンスデータを分析対象とし、実証研究を行っています。</p>

<div class="cards">
  <div class="card">
    <h3>計量ファイナンス</h3>
    <p>株式市場データや資産価格データを用いて、投資リスクの定量分析、資産価格の予測モデル開発、市場アノマリーの検証などに取り組みます。</p>
  </div>
  <div class="card">
    <h3>テキストデータ分析</h3>
    <p>ニュース記事や企業開示資料、SNSなどのテキストを自然言語処理で解析し、金融市場との関係を実証的に分析します。</p>
  </div>
  <div class="card">
    <h3>機械学習・AIの金融応用</h3>
    <p>機械学習や深層学習をファイナンスに応用し、資産価格の予測や説明可能なAI、気候変動リスクの計測などに取り組みます。</p>
  </div>
</div>

## News

<ul class="news-list">
{% for n in site.data.news %}
  <li><span class="news-date">{{ n.date }}</span><span>{% if n.link %}<a href="{{ n.link | relative_url }}">{{ n.text }}</a>{% else %}{{ n.text }}{% endif %}</span></li>
{% endfor %}
</ul>

## 学生募集

<div class="cards">
  <a class="card card-link" href="{{ '/student/seminar/' | relative_url }}">
    <h3>学部ゼミ紹介</h3>
    <p>ゼミを探している学部生の方へ</p>
  </a>
  <a class="card card-link" href="{{ '/student/lab/' | relative_url }}">
    <h3>大学院のご案内</h3>
    <p>大学院進学をお考えの方へ</p>
  </a>
</div>

## 五島研究室を選ぶ理由

<ul class="checklist">
  <li><strong>対外発表</strong>：学部生も希望に応じてデータ分析コンペや学会発表に挑戦できます（SDSC2024、CSSJ2025で発表実績）</li>
  <li><strong>自由な研究スタイル</strong>：コアタイムなし。自身の生活リズムに合わせて研究に取り組めます</li>
  <li><strong>手厚い経費サポート</strong>：研究経費（PC代・データ購入費・学会参加費・発表旅費など）は研究室の予算で可能な限り負担します</li>
</ul>

{% include contact.html text="共同研究・取材・講演のご相談や、大学院進学の事前相談など、下記のメールアドレスへお気軽にご連絡ください。" %}
