[Wiki Home](https://github.com/XinYang-Pan/Misc/wiki)




| Table Name        | Schema  | Engine |
|:------------------|:--------|:-------|
| HEDGING_EXECUTION | HEDGING | InnoDB |



| No | Name            | Desc | Type      | Size | Decimal Digits | PK | FK | NOT NULL | Default           | Enum | Charset | Comment        |
|:---|:----------------|:-----|:----------|:-----|:---------------|:---|:---|:---------|:------------------|:-----|:--------|:---------------|
| 1  | ID              |      | BIGINT    | 19   | 0              | Y  |    | NO       |                   |      |         | AUTO_INCREMENT |
| 2  | LP_ID           |      | SMALLINT  | 5    | 0              |    |    | NO       |                   |      |         |                |
| 3  | BOOK_ID         |      | INT       | 10   | 0              |    |    | NO       |                   |      |         |                |
| 4  | SYMBOL_ID       |      | SMALLINT  | 5    | 0              |    |    | NO       |                   |      |         |                |
| 5  | SOURCE_ID       |      | BIGINT    | 19   | 0              |    |    | NO       |                   |      |         |                |
| 6  | COMPANY_ID      |      | TINYINT   | 3    | 0              |    |    | NO       |                   |      |         |                |
| 7  | LP_ORDER_ID     |      | VARCHAR   | 32   |                |    |    | YES      |                   |      |         |                |
| 8  | LP_SYMBOL_ID    |      | INT       | 10   | 0              |    |    | NO       |                   |      |         |                |
| 9  | LP_EXECUTE_ID   |      | VARCHAR   | 64   |                |    |    | YES      |                   |      |         |                |
| 10 | SIDE            |      | TINYINT   | 3    | 0              |    |    | YES      |                   |      |         |                |
| 11 | SETTLE_DATE     |      | DATE      | 10   |                |    |    | YES      |                   |      |         |                |
| 12 | ORDER_PRICE     |      | DECIMAL   | 15   | 9              |    |    | YES      |                   |      |         |                |
| 13 | EXECUTE_DATE    |      | DATE      | 10   |                |    |    | NO       |                   |      |         |                |
| 14 | EXECUTE_TIME    |      | BIGINT    | 19   | 0              |    | Y  | NO       |                   |      |         |                |
| 15 | EXECUTE_PRICE   |      | DECIMAL   | 15   | 9              |    |    | YES      |                   |      |         |                |
| 16 | EXECUTE_VOLUME  |      | DECIMAL   | 20   | 2              |    |    | YES      |                   |      |         |                |
| 17 | EXECUTE_AMOUNT  |      | DECIMAL   | 20   | 2              |    |    | YES      |                   |      |         |                |
| 18 | EXECUTE_RESULT  |      | TINYINT   | 3    | 0              |    | Y  | YES      |                   |      |         |                |
| 19 | EXECUTE_COMMENT |      | VARCHAR   | 256  |                |    |    | YES      |                   |      |         |                |
| 20 | VERSION         |      | INT       | 10   | 0              |    |    | NO       | 1                 |      |         |                |
| 21 | INSERT_DATETIME |      | TIMESTAMP | 19   |                |    |    | YES      |                   |      |         |                |
| 22 | UPDATE_DATETIME |      | TIMESTAMP | 19   |                |    |    | NO       | CURRENT_TIMESTAMP |      |         |                |

