# game_bosyu


## データ設計

- 投稿
  - 機種
    - switch, ps, xbox, pc

  - ID
    - Discord, PSID

  - 目的
    - フレンド
    - ランク
    - カジュアル
    - 練習
    - 競技
    - その他
- contacts
  - id
  - name, string, unique
  - コメント
    - text(50文字以内)


## テーブル設計

- games
  - id
  - title

- machines
  - id
  - name, string, unique

- destinations
  - id
  - name, string, unique

- contacts
  - id
  - name, string, unique

- contact_posts
  - id
  - contanct_id
  - post_id
  - content

- posts
  - columns
    - id
    - game_id, integer
    - contact_id, integer
    - machine_id, integer
    - destination_id, integer
    - comments, text


# 掲示板表示


- 表示No      , 日付, コメント
  機種名・目的      , 連絡先ID　　　

 
