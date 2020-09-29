# SugoiAir Toy Project DataBase CREATE SQL

```sql 
-- 코드 테이블
CREATE TABLE `tbl_code` (
  `c_no` int NOT NULL AUTO_INCREMENT COMMENT 'INDEX',
  `c_cg_id` int NOT NULL COMMENT '그룹코드 ID',
  `c_id` int NOT NULL COMMENT '코드 아이디',
  `c_name` varchar(255) CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci NOT NULL COMMENT '코드 이름',
  PRIMARY KEY (`c_no`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;

CREATE TABLE `tbl_code_group` (
  `cg_id` int NOT NULL AUTO_INCREMENT COMMENT '그룹코드',
  `cg_name` varchar(255) CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci NOT NULL COMMENT '그룹코드 이름',
  `cg_remark` varchar(255) CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci NOT NULL COMMENT '비고',
  PRIMARY KEY (`cg_id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;

CREATE TABLE `tbl_users` (
  `u_no` int NOT NULL AUTO_INCREMENT COMMENT 'INDEX',
  `u_id` varchar(255) CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci NOT NULL COMMENT '사용자 아이디',
  `u_password` varchar(255) CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci NOT NULL COMMENT '사용자 비밀번호',
  `u_name` varchar(255) CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci NOT NULL COMMENT '사용자 이름',
  PRIMARY KEY (`u_no`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;


```