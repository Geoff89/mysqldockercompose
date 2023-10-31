`mkdir mysql-project`

`cd mysql-project`

`touch docker-compose.yml`

`docker-compose up -d`

`docker ps`

`mysql -h 127.0.0.1 -P 3306 -u root -p`

CREATE TABLE users (
    id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY,
    first_name VARCHAR(30) NOT NULL,
    last_name VARCHAR(30) NOT NULL,
    email VARCHAR(50),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

INSERT INTO users (first_name, last_name, email)
VALUES ('Christian', 'Schou', 'chsc@christian-schou.dk');

SELECT * FROM users;
