# 運用フロー

## 情報の収集

一週間かけてiOS関連の情報を収集します。

## 記事の執筆

以下のルールで記事を執筆します。

- ファイル名: `999-YYYYMMDD.md`
  - ファイル名がそのままURLのパスになる
  - 3桁の連番に投稿日をハイフン区切りで付ける
  - 例: `001-20220404.md`
- ファイル内のヘッダー
  - date: `YYYY-MM-DD hh:mm`
    - 日時は投稿日の9時とする
    - 例: `date: 2022-04-04 09:00`
  - description: `999 YYYY-MM-DD`
    - ファイル名と同様の連番と日時とする
    - 例: `001 2022-04-04`
  - tags: `ios` や `swift` などを自由に付ける
    - すべて小文字でカンマ+半角スペース区切りとする
    - 2単語以上の場合はハイフンで繋げる
    - 例: `apple, swift, ios, github-actions`
- ファイル内の本文
  - 見出し1
    - `999 YYYY-MM-DD` とする
    - descriptionと同様とする
    - 例: `001 2022-04-04`
  - 見出し2以降
    - 自由に付ける

## PRの作成

記事を執筆したら `main` ブランチへPRを作成します。

## PRのマージ

以下の条件を満たしたらPRをマージします。

- CIが通っている
- 1人以上Approveしている
- コメントがすべて解決している

毎週月曜日の9:00に自動でGitHub Pagesにホスティングされます。

## Twitterでの周知

GitHub Pagesにホスティングされたら、公式アカウント（[@ios_osushi](https://twitter.com/ios_osushi)）で記事の投稿を周知します。

内容は以下とします。

```
iOS Osushi🍣がiOS関連ニュースの第999回をお届けします。
https://ios-osushi.github.io/posts/999-YYYYMMDD/
#ios_osushi
```
