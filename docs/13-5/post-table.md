| カラム名    | データ型     | 制約                  | 説明                        |
| :---------- | :----------- | :-------------------- | :-------------------------- |
| id          | BIGINT       | PRIMARY KEY           | 投稿を1件ずつ区別する番号   |
| user_id     | BIGINT       | NOT NULL, FOREIGN KEY | 投稿ユーザー                |
| category_id | BIGINT       | NOT NULL, FOREIGN KEY | カテゴリ                    |
| title       | VARCHAR(255) | NOT NULL              | タイトル文字数は255文字制限 |
| content     | TEXT         | NOT NULL              | 本文文字数は1000文字制限    |
| created_at  | TIMESTAMP    | -                     | 投稿日時                    |
| updated_at  | TIMESTAMP    | -                     | 更新日時                    |
