# Bamboo


## Run Bamboo container;
docker run \
  --detach \
  --name bamboo \
  --env DOCKER_GID=999 \
  --env JVM_MINIMUM_MEMORY=512m \
  --env JVM_MAXIMUM_MEMORY=1024m \
  --volume /var/run/docker.sock:/var/run/docker.sock \
  --volume /usr/bin/docker:/usr/bin/docker:ro \
  --volume /storage/bamboo:/var/atlassian/application-data/bamboo \
  --publish 8085:8085 \
  --publish 54663:54663 \
  containerstack/bamboo:6.2.3

ʕ•͡•ʔ
