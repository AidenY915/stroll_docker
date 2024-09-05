cd stroll_tomcat <br/>
docker image build -t stroll_tomcat . <br/>
cd .. <br/>
<br/>
cd stroll_mysql <br/>
docker image build -t stroll_mysql . <br/>
cd .. <br/>
<br/>
docker-compose up<br/>
<br/>
open "http://localhost:8081/stroll_docker/main"
