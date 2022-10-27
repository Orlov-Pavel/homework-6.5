FROM centos:7

COPY ./files/elasticsearch-8.4.3-linux-x86_64.tar.gz ./elasticsearch-8.4.3-linux-x86_64.tar.gz

RUN tar -xzf elasticsearch-8.4.3-linux-x86_64.tar.gz && \
    rm elasticsearch-8.4.3-linux-x86_64.tar.gz

COPY ./files/elasticsearch.yml /elasticsearch-8.4.3/config/elasticsearch.yml

RUN useradd elastic && \
    chown -R elastic:elastic elasticsearch-8.4.3 && \
    mkdir /var/lib/elastic && \
    chown -R elastic:elastic /var/lib/elastic

USER elastic

WORKDIR /elasticsearch-8.4.3

CMD ["./bin/elasticsearch"]