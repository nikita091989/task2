# 
A [docker-compose](https://docs.docker.com/compose/) sample to start `MySQL` database and phpmyadmin

# How to use?

1. Clone the project:

  ```shell
    $ git clone https://github.com/nikita091989/task2.git
  ```

2. Start `MySql and phpmyadmin` via [docker-compose](https://docs.docker.com/compose/) in terminal:

  ```shell
    $ cd ./task2
    $ docker-compose up -d
  ```
3. Connect to the MySQL:
  ```
    # Enter in the docker container
    $ docker exec -it mysqldb1 bash
    # Connect to mysql service, and enter in password 123456
    $ mysql -h 127.0.0.1 -u user -P 3306 -p
  ```
4. Connect to the phpmyadmin:
  ```
    # Enter in the docker container
    $ docker exec -it admindb1 bash
  ```
5. Other commands maybe needed:
  ```
    # you can stop service by the command
    $ docker stop mysqldb1
    $ docker stop 
    # you can start service by the command
    $ docker start mysqldb1
    $ docker start admindb1
    # you can restart service by the command
    $ docker restart mysqldb1
    $ docker restart admindb1
  ```
6. Other:
  ```
    # you can set up database variables in the .env file
  ```


