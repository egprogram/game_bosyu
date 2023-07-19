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

- posts
  - columns
    - id
    - game_id, integer
    - contact_id, integer
    - machine_id, integer
    - destination_id, integer
    - comments, text
    - friend_id, text

