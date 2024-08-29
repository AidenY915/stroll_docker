FROM mysql:latest

# 초기 SQL 스크립트를 초기화 스크립트 폴더로 복사
COPY stroll_table.sql /docker-entrypoint-initdb.d/stroll_table.sql

EXPOSE 3306

# MySQL root 사용자 비밀번호 설정
ENV MYSQL_ROOT_PASSWORD=1234
