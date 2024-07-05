# Demo Docker Registry

## Авторизация в сервисе 
`docker login  -u ${USER_LOGIN}  -p ${PSWD}  registry.smalvi.ru`



## сборка

`docker --log-level=debug build --pull --file=api/docker/common/postgres-backup/Dockerfile --tag=registry.smalvi.ru/auction-api-postgres-backup:${IMAGE_TAG} api/docker/common`


## push

`docker push registry.smalvi.ru/${IMAGE_NAME}:{IMAGE_TAG}`


IMAGE_NAME   -  имя ```пример - auction-api-postgres-backup```  и одновременно имя\расположение а репе