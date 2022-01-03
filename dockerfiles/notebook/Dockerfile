# http://serverarekore.blogspot.com/2018/04/dockerjupyter-notebookpostgresql.html?m=1
# docker build -t scipy-notebook-pg .

from jupyter/scipy-notebook

env TZ=Asia/Tokyo

user root

run apt-get update \
  && apt-get -y install libpq-dev python-dev \
  && pip install psycopg2-binary \
  && apt-get clean

user $NB_UID
