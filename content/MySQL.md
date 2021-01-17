## 본질
* ::Input::
	* *C*reate
	* *U*pdate
	* *D*elete
* ::Output::
	* *R*ead

### MySQL 접속

```bash
MySQL - root password asdfasdf
$ cd /usr/local/mysql/bin
$ ./mysql -uroot -pasdfasdf
```

### SQL과 테이블 구조

* 스키마: DB내에 어떤 구조로 데이터가 저장되는가를 나타내는 데이터베이스 구조를 스키마라고 함

### Table 생성
```bash
mysql> create table topic(
    id INT(11) NOT NULL AUTO_INCREMENT,
    title VARCHAR(100) NOT NULL,
    description TEXT NULL,
    created DATETIME NOT NULL,
    author VARCHAR(15) NULL,
    profile VARCHAR(200) NUll,
	  PRIMARY KEY(id)
    );
```

### CRUD

#### Create
```bash
$ insert into topic (title,description,created,author,profile) values('MySQL','MySQL is ...',NOW(),'kevin','developer');
```

#### Read
```bash
$ select * from topic;
```

#### Update
```bash
$ update topic set description='Oracle is updated ...' where id=2;
```

#### Delete
```bash
$ delete from topic where id=5;
```

### Join

### Workbench and MySQL monitor
```bash
$ cd /usr/local/mysql/bin
$ ./mysql -uroot -p -h127.0.0.1 #-h는 host를 의미
$ ./mysql -uroot -pasdfasdf #-h를 생략가능
```

### 생각해 볼 주제
index (색인),  model (정규화, 비정규화, 역정규화), backup, Clowd(AWS RDS)

#MySQL #Database #workbench #MySQL_Monitor
