# SugoiAir Toy Project DataBase CREATE SQL

```sql 
-- 코드 테이블
CREATE TABLE `tbl_code` (
  `C_NO` int NOT NULL AUTO_INCREMENT COMMENT 'INDEX',
  `C_CG_ID` int NOT NULL COMMENT '그룹코드 ID',
  `C_ID` int NOT NULL COMMENT '코드 아이디',
  `C_NAME` varchar(255) CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci NOT NULL COMMENT '코드 이름',
  PRIMARY KEY (`C_NO`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;
-- 코드그룹 테이블
CREATE TABLE `tbl_code_group` (
  `CG_ID` int NOT NULL AUTO_INCREMENT COMMENT '그룹코드',
  `CG_NAME` varchar(255) CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci NOT NULL COMMENT '그룹코드 이름',
  `CG_REMARK` varchar(255) CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci NOT NULL COMMENT '비고',
  PRIMARY KEY (`CG_ID`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;

-- 사용자 테이블
CREATE TABLE `tbl_users` (
  `U_NO` int NOT NULL AUTO_INCREMENT COMMENT 'INDEX',
  `U_ID` varchar(255) CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci NOT NULL COMMENT '사용자 아이디',
  `U_PASSWORD` varchar(255) CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci NOT NULL COMMENT '사용자 비밀번호',
  `U_NAME` varchar(255) CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci NOT NULL COMMENT '사용자 이름',
  PRIMARY KEY (`U_NO`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;

```