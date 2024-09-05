FROM mysql:latest

# 초기 SQL 스크립트를 초기화 스크립트 폴더로 복사
COPY stroll_table.sql /docker-entrypoint-initdb.d/stroll_table.sql
#lower_case_table_names=1 설정을 위한 파일
COPY ./my.cnf /etc/mysql/conf.d/my.cnf
# 파일 권한 변경(mySQL 데몬이 모든 사용자가 수정할 수 있는 파일은 사용하지 않음)
RUN chmod 644 /etc/mysql/conf.d/my.cnf

EXPOSE 3306

# MySQL root 사용자 비밀번호 설정
ENV MYSQL_ROOT_PASSWORD=1234