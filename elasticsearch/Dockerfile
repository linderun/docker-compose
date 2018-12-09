FROM docker.elastic.co/elasticsearch/elasticsearch:6.4.3

LABEL maintainer="Darren Lin <linderun@linderun.com>"

###########################################################################
# elasticsearch-analysis-ik:
###########################################################################

ARG INSTALL_ELASTICSEARCH_ANALYSIS_IK=false

RUN if [ ${INSTALL_ELASTICSEARCH_ANALYSIS_IK} = true ]; then \
    cd /usr/share/elasticsearch && \
    echo y | ./bin/elasticsearch-plugin install https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v6.4.3/elasticsearch-analysis-ik-6.4.3.zip \
;fi

EXPOSE 9200 9300
