# テーブル設計

## usersテーブル

| Column     | Types  | Options  |
| ---------- | ------ | -------- |
| email      | string | NOT NULL |
| password   | string | NOT NULL |
| name       | string | NOT NULL |
| profile    | text   | NOT NULL |
| occupation | text   | NOT NULL |
| position   | text   | NOT NULL |

## prototypesテーブル

| Column     | Types      | Options  |
| ---------- | ---------- | -------- |
| title      | string     | NOT NULL |
| catch_copy | text       | NOT NULL |
| concept    | text       | NOT NULL |
| image      |            |          |
| user       | references |          |

## commentsテーブル

| Column    | Types     | Options  |
| --------- | --------- | -------- |
| text      | text      | NOT NULL |
| user      | references |          |
| prototype | references |          |