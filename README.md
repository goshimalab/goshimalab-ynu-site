# 五島研究室ホームページ

GitHub Pages（Jekyll）で公開している、横浜国立大学・五島研究室のWebサイトです。
（旧サイト: https://sites.google.com/view/goshima-lab ）

## よくある更新

| やりたいこと | 編集するファイル |
|---|---|
| News を追加 | `_data/news.yml`（一番上に追記） |
| 研究実績を追加 | `_data/publications.yml` |
| メニュー項目を変更 | `_data/navigation.yml` |
| 各ページの本文 | `index.md`（ホーム）, `seminar.md`（学部ゼミ）, `graduate.md`（大学院）, `publications.md`, `teacher.md` |
| メールアドレス等 | `_config.yml` |
| デザイン | `assets/css/style.css` |

GitHub上でファイルを直接編集して commit するだけで、1〜2分後にサイトへ反映されます。

### News の書き方（`_data/news.yml`）

```yaml
- date: "2026.03"
  text: ○○学会でゼミ生が研究発表を行いました
  link: /publications/   # 任意
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

## 公開手順（初回のみ）

1. GitHubで新しいリポジトリを作成し、このフォルダを push する
2. リポジトリの **Settings → Pages** で、Source を「Deploy from a branch」、Branch を `main` / `(root)` にする
3. リポジトリ名が `<ユーザー名>.github.io` でない場合は、`_config.yml` の `baseurl` を `"/<リポジトリ名>"` に変更する

## ローカルでのプレビュー（任意）

```bash
bundle install
bundle exec jekyll serve
```

http://localhost:4000 で確認できます。
