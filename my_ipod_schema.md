# My iPod Schema

**Genres**

| PK   | id   | Integer |
| ---- | ---- | ------- |
|      | name | String  |

**Artists**

| PK   | id            | Integer |
| ---- | ------------- | ------- |
|      | name          | String  |
|      | bio           | String  |
|      | grammy_amount | Integer |
|      | year_started  | Integer |

**Albums**

| PK   | id            | Integer |
| ---- | ------------- | ------- |
|      | name          | String  |
|      | year_released | Integer |
|      | label         | String  |
| FK   | genre_id      | Integer |
| FK   | artist_id     | Integer |

**Songs**

| PK   | id       | Integer |
| ---- | -------- | ------- |
|      | name     | String  |
|      | length   | String  |
| FK   | album_id | Integer |

