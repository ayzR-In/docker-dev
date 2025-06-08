# Env Setup

A minimal sandbox cluster running via docker-compose (1 master, 1 worker) as described in this medium article.

TLDR: I'm not reading that article

export JAVA_HOME=/path/to/jre
docker pull bitnami/spark:3.5.1
conda create -n pyspark-311 python=3.11 pyspark=3.5.1
export HOST_IP=<YOUR IPV4 IP>
docker-compose up --build
conda activate pyspark-311 && python hello-pyspark.py