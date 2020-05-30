FROM postgres:12

RUN apt-get update; \
    apt-get install -y pgxnclient \
                       postgresql-server-dev-12 \
                       build-essential \
                       make; \
    apt-get clean; \
    rm -rf /var/lib/apt/lists/*

RUN pgxn install postgresql_anonymizer
