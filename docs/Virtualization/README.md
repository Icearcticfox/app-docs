### Docker
Сети в докере
 - https://stackoverflow.com/questions/41847656/network-not-manually-attachable-when-running-one-off-command-against-docker-sw

**В чем разница между CMD и ENTRYPOINT:**

Флаг --entrypoint может быть использован, чтобы переопределить инструкцию ENTRYPOINT:

`docker run --entrypoint [my_entrypoint] test  `

Все, что следует после названия образа в команде docker run, переопределяет инструкцию CMD:

`docker run test [command 1] [arg1] [arg2]'`

https://habr.com/ru/company/southbridge/blog/329138/



####Multi arch docker 
https://www.docker.com/blog/getting-started-with-docker-for-arm-on-linux/
buildex
builder image https://hub.docker.com/r/docker/binfmt/tags

https://medium.com/@artur.klauser/building-multi-architecture-docker-images-with-buildx-27d80f7e2408


https://hungpham2511.github.io/2021/02/06/docker-arm-support-with-buildx-and-simulator.html


enble experemental
https://www.deploycontainers.com/2021/09/27/enable-experimental-features-on-docker-desktop/