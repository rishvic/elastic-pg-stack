FROM docker.elastic.co/logstash/logstash:8.7.0

COPY ./postgresql-42.6.0.jar logstash-core/lib/jars/postgresql-42.6.0.jar
COPY ./pipeline-movie.conf config/pipeline-movie.conf

CMD bin/logstash -f config/pipeline-movie.conf
