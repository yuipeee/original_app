# テーブル設計

## menus テーブル

| Column             | Type       | Options                        |
| ------------------ | ---------- | ------------------------------ |
| style              | string     | null: false                    |
| material           | string     | null: false                    |
| feeling            | string     | null: false                    |
| name_id            | references | null: false, foreign_key: true |

### Association

- has_many :foods

## items テーブル

| Column           | Type       | Options                        |
| ---------------- | ---------- | ------------------------------ |
| name             | string     | null: false                    |

### Association

- has_one :menu
