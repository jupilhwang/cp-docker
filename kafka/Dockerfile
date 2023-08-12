FROM confluentinc/cp-server:7.4.1

RUN echo "==> Createing Logs Dir" \
	&& mkdir -p /var/log/kafka \
	&& chmod -R ag+w /var/log/kafka

VOLUME ["/var/lib/${COMPONENT}/data", "/etc/${COMPONENT}/secrets", "/var/log/kafka"] 

COPY log4j.properties.template /etc/confluent/docker/log4j.properties.template
