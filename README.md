# HW 03

## Task 01

```bash

cd task1

# 1. run postgres container
sudo docker run --name hw03_db -p 5432:5432 -e POSTGRES_PASSWORD=123456 -d postgres

# 2. create tables
python create_tables.py

# 3. add data
python seed.py

# 4. execute queries
python execute_queries.py

```

## Task 02

``` bash

cd task2

sudo docker run --name hw03_mongodb -d -p 27017:27017 mongo

python create_db.py

python main.py

```