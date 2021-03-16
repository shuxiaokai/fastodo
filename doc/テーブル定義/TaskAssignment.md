# タスクアサインテーブル定義

## task_assignment
|カラム名|型|制約|コメント|
|---|---|---|---|
|id|BIGINT UNSIGNED (20)|PK|ID|
|task_id|BIGINT UNSIGNED (20)|NOT NULL FK: task.id|タスクID|
|user_id|BIGINT UNSIGNED (20)|NOT NULL FK: user.id|ユーザID|
|is_deleted|TINYINT (1)|NOT NULL|論理削除カラム|
|created_at|DATETIME|NOT NULL|作成日時|
|updated_at|DATETIME|NOT NULL|作成日時|