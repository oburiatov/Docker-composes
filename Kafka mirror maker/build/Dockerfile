FROM confluentinc/cp-kafka:6.1.0

USER root

COPY connect-mirror-maker /bin/
COPY mm2-prefixless-policy-1.0.0-SNAPSHOT.jar /usr/share/java/kafka/
RUN chmod a+x /bin/connect-mirror-maker

CMD ["/bin/connect-mirror-maker", "/etc/kafka/config/connect-mirror-maker.properties"]

