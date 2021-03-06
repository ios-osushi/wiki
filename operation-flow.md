# 運用フロー

## 情報の収集

1週間かけてiOS関連の情報を収集します。

## 作業ブランチなどの作成

[Create post](https://github.com/ios-osushi/website/actions/workflows/create_post.yml) を実行し、作業ブランチ・Markdownファイル・Draft PRを作成します。

## 記事の執筆

以下のルールで記事を執筆します。

- ファイル名: `999-YYYYMMDD.md`
  - ファイル名がそのままURLのパスになる
  - 3桁の連番に投稿日をハイフン区切りで付ける
  - 例: `001-20220404.md`
- ファイル内のヘッダー
  - date: `YYYY-MM-DD hh:mm`
    - 投稿日の9時とする
    - 例: `date: 2022-04-04 09:00`
  - description: 記事の概要を自由に書く
    - 見出し2を読点（ `、` ）で繋げるのを推奨とする
    - 例: `swift-async-algorithms プロトタイプリリース、リーダーアプリのアカウント管理についての更新`
  - tags: `ios` や `swift` などを自由に付ける
    - すべて小文字でカンマ+半角スペース区切りとする
    - 2単語以上の場合はハイフンで繋げる
    - 例: `apple, swift, ios, github-actions`
- ファイル内の本文
  - 見出し1
    - `999 YYYY-MM-DD` とする
    - 連番と投稿日はファイル名と合わせる
    - 例: `001 2022-04-04`
  - 見出し2以降
    - テンプレートに沿って付ける

## レビュー依頼

記事を執筆したら概要を記述してレビュアーを設定し、PRのDraftを解除します。

## PRのマージ

以下の条件を満たしたらPRをマージします。

- CIが通っている
- 1人以上Approveしている
- できる限りコメントが解決している

毎週月曜日の9:00頃に自動でGitHub Pagesにホスティングされます。

## Twitterでの周知

GitHub Pagesにホスティングされたら、公式アカウント（[@ios_osushi](https://twitter.com/ios_osushi)）で記事の投稿を周知します。

内容は以下とします。

```
iOS関連ニュースの第999回をお届けします🍣

{description}

https://ios-osushi.github.io/posts/999-YYYYMMDD/
#ios_osushi
```

例

```
iOS関連ニュースの第001回をお届けします🍣

swift-async-algorithms プロトタイプリリース、リーダーアプリのアカウント管理についての更新、iOS 15.4.1リリース、iPadOS 15.4.1リリース、macOS 12.3.1リリース、watchOS 8.5.1リリース

https://ios-osushi.github.io/posts/001-20220404/
#ios_osushi
```
