# 五島研究室ホームページ

GitHub Pages（Jekyll）で公開している、横浜国立大学・五島研究室のWebサイトです。
（旧サイト: https://sites.google.com/view/goshima-lab ）

GitHub上でファイルを直接編集して commit するだけで、1〜2分後にサイトへ反映されます。

## 1. サイトの構造

3つの層に分かれています。**本文を直すときは 1-2 の `.md`、繰り返し出てくるデータは 1-3 の `_data/`** だけを触れば済みます。

```
_layouts/default.html   全ページ共通の骨格（これ1つだけ）
  ├ head（title / description / OG / favicon / フォント / CSS）
  ├ header.html         ロゴ + メニュー + お問い合わせボタン
  ├ hero.html           front matter に hero: があるページだけ表示
  ├ main > article      ← 各 .md の本文がここに入る
  └ footer.html         所属・メール・リンク一覧・YNUロゴ

*.md                    各ページの中身（8ページ）
_data/*.yml             メニュー・News・研究実績（繰り返しデータ）
assets/css/style.css    デザインのすべて（1ファイル）
assets/img/             ロゴ・favicon
```

### 1-1. ページ一覧

| ページ | ファイル | URL | メニュー |
|---|---|---|---|
| ホーム | `index.md` | `/` | ホーム |
| ファイナンスとは | `finance.md` | `/finance/` | ファイナンスとは |
| 学部ゼミ | `seminar.md` | `/seminar/` | 学部ゼミ |
| 大学院 | `graduate.md` | `/graduate/` | 大学院 |
| 社会人の方へ | `professional.md` | `/professional/` | 大学院 ＞ 社会人の方へ |
| 教員紹介 | `teacher.md` | `/teacher/` | 教員紹介 |
| 企業の方へ | `industry.md` | `/industry/` | 企業の方へ |
| Graduate School（英語） | `graduate-en.md` | `/en/graduate/` | English |

英語版ページは front matter に `lang: en` を書きます。これだけで、メニュー・フッター・定型文が英語に切り替わります。

### 1-2. front matter がページの設計書

本文を書かなくても、`.md` の先頭（`---` で囲んだ部分）の指定だけで見た目が決まります。

| 指定 | 役割 |
|---|---|
| `permalink: /seminar/` | 公開URL |
| `title:` / `description:` | ブラウザのタブ名・検索結果の説明文 |
| `eyebrow:` | 見出しの上に出る小さな英語ラベル |
| `hero:` / `hero_lead:` / `hero_buttons:` | ページ上部の大見出し・リード文・ボタン（`hero:` を書かないと簡易見出しになります） |
| `hero_style: navy` | ヒーローの配色 |
| `theme: friendly` | ページ全体の配色（学部ゼミのみ使用） |
| `has_contact: true` | 本文末に連絡先ボックスを置くページ（ヘッダーの「お問い合わせ」のリンク先が切り替わります） |
| `lang: en` | 英語ページ |

### 1-3. 共通部品（`_includes/`）

| ファイル | 役割 | 呼び出し方 |
|---|---|---|
| `header.html` | メニュー。現在のページを自動でハイライト | レイアウトが自動で挿入 |
| `hero.html` | ページ上部の大見出し | `hero:` があるページのみ自動 |
| `footer.html` | 連絡先とリンク一覧 | レイアウトが自動で挿入 |
| `contact.html` | 本文末の連絡先ボックス | `{% include contact.html title="…" text="…" %}` |
| `icon.html` | SVGアイコン | `{% include icon.html name="chart" %}` |
| `student-pubs.html` | `publications.yml` を年ごとに整形 | `{% include student-pubs.html %}` |

`icon.html` で使える `name`（全18種）: `ai` `arrow` `award` `book` `briefcase` `chart` `chat` `clock` `code` `home` `leaf` `mic` `moon` `paper` `plane` `team` `text` `yen`

## 2. よくある更新

| やりたいこと | 編集するファイル |
|---|---|
| News を追加 | `_data/news.yml`（一番上に追記） |
| 学生の研究成果を追加 | `_data/publications.yml` |
| メニュー項目を変更 | `_data/navigation.yml`（英語版は `_data/navigation_en.yml`） |
| 各ページの本文 | 上の「ページ一覧」の該当ファイル |
| メールアドレス・サイト名 | `_config.yml` |
| デザイン | `assets/css/style.css` |

### News の書き方（`_data/news.yml`）

```yaml
- date: "2026.03"
  text: ○○学会でゼミ生が研究発表を行いました
  link: /seminar/#results   # 任意
```

### 研究実績の書き方（`_data/publications.yml`）

```yaml
- year: 2026
  items:
    - authors: 氏名・五島圭一
      title: 論文タイトル
      venue: 学会名
      place: 東京
      date: 2026年3月
```

### メニューの書き方（`_data/navigation.yml`）

並べた順に表示されます。`children:` を付けると、PCではドロップダウン、スマホでは字下げした子項目になります。

```yaml
- title: 大学院
  url: /graduate/
  children:
    - title: 大学院の案内
      url: /graduate/
    - title: 社会人の方へ
      url: /professional/
```

## 3. 公開手順（初回のみ）

1. GitHubで新しいリポジトリを作成し、このフォルダを push する
2. リポジトリの **Settings → Pages** で、Source を「Deploy from a branch」、Branch を `main` / `(root)` にする
3. リポジトリ名が `<ユーザー名>.github.io` でない場合は、`_config.yml` の `baseurl` を `"/<リポジトリ名>"` に変更する

## 4. ローカルでのプレビュー（任意）

```bash
bundle install
bundle exec jekyll serve
```

http://localhost:4000 で確認できます。

## 5. その他

- `WEB用（RGB）_JPEGデータ/` は大学から配布されたロゴの元データです。`.gitignore` と `_config.yml` の `exclude` の両方に入れてあるため、GitHubにもサイトにも公開されません（手元にだけ残ります）。サイトで使うのは `assets/img/` の加工済み画像です。
