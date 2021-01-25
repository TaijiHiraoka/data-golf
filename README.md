# data-golf
- アプリ概要｜ゴルフショットデータ管理
- ハードウェア｜スイングトレーナー　https://www.yupiteru.co.jp/products/golf_trainer/gst-5arc/
- インプットデータ｜csv

# Data Base
## usersテーブル
|Column    |Type   |Options    |
|----------|-------|-----------|
|user_id   |integer|null: false|
|nickname  |strings|null: false|

### Assosiation
- has_many :datas

## datasテーブル
|Column    |Type   |Options    |
|----------|-------|-----------|
|club_num  |strings|null: false|
|head_speed|integer|null: false|
|distance  |integer|null: false|
|ball_speed|integer|null: false|
|meat_rate |integer|null: false|

### Assosiation
- belongs_to :user
