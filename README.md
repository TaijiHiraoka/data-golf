# data-golf
- アプリ概要｜ゴルフデータ管理
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
|Club      |strings|null: false|
|Head_speed|integer|null: false|
|distance  |integer|null: false|
|Ball_speed|integer|null: false|
|Meat_rate |integer|null: false|

### Assosiation
- belongs_to :user
