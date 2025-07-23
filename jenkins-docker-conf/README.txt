#installation de image docker java21/maven:
docker image pull maven:3.9-amazoncorretto-21-debian

#verification de l'image docker java21/maven:
docker container run -t -i maven:3.9-amazoncorretto-21-debian bash
# java --version
# mvn --version
# exit

====================

Vérification du container docker correspondant au controleur Jenkins:

docker container exec -ti jenkins_controller_container bash