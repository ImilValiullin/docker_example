# docker
`sudo docker ps` - список запущенных контейнеров 
sudo docker images 
`sudo docker run -p 8888:8888 jupyter/scipy-notebook:6b49f3337709` - звпустить контейнер с jupyter   
`sudo docker exec -it fb3a93d7c30c bash `- заходим в FS контейнера   
`sudo docker stop fb3a93d7c30c` - остановить контейнер   
`sudo docker cp wine.data 47df1c36432a:/home/jovyan/wine.data` - перекинуть данные в контейнер  

`sudo docker build -t notebook .` - сборка нового образа с учетом Dockerfile

`sudo docker run -v /home/imil/docker_example:/home/jovyan/ -p 8888:8888 notebook` - запуск новой сборки

`sudo docker volume ls` - просмотр вольюмов

# docker-compose
`sudo docker-compose up --build` - сделать сборку и поднять контейнеры

`sudo docker-compose down` - удалить контейнеры


sudo docker system prune (-a)
