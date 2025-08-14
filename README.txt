Ce référentiel git comporte une configuration de Jenkins pour un fonctionnement simple en mode "dind" (docker in docker):
Environnement cible : WSL2/windows_10ou_11
NB: la configuration docker-compose/Jenkins/
    - installera automatiquement les plugins fondamentaux (git, docker , …)

====
rappel pour tester une image docker:
docker container run -p 8282(host):8181(internal) --name xyz_container xxx/yyy_image_name:tag
et
-ti pour mode interactif
-d pour mode détaché
et
docker container exec -ti xyz_container sh
pour tester un conteneur existant

==== 
pour mongo:8.0.12

docker container run -p 27018:27017 --name my_mongo_container -d mongo:8.0.12
et
docker container exec -ti my_mongo_container sh