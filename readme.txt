Running Maria DB

docker run --name some-mariadb -e MYSQL_ROOT_PASSWORD=my-secret-pw -d mariadb:latest


Accessing Maria DB

1. Find IP of Maria DB - docker containser inspect some-mariadb

2. docker run -it --network bridge --rm mariadb mysql -h <ip from 1 above> -u root -p 
