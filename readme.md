cd stroll_tomcat
docker image build -t stroll_tomcat .
cd ..

cd stroll_mysql
docker image build -t stroll_mysql .
cd ..

docker-compose up
