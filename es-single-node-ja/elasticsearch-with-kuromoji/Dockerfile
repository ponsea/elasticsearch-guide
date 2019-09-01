ARG ES_IMG_VERSION=7.3.1

FROM elasticsearch:$ES_IMG_VERSION
MAINTAINER ponsea

# install kuromoji Analysis Plugin
RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install analysis-kuromoji

EXPOSE 9200 9300

ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
CMD ["eswrapper"]
