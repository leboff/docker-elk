ARG ELK_VERSION

# https://github.com/elastic/logstash-docker
FROM docker.elastic.co/logstash/logstash-oss:${ELK_VERSION}

COPY logstash-input-sfdc_elf-1.0.2.gem /plugins/
# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json

RUN logstash-plugin install /plugins/logstash-input-sfdc_elf-1.0.2.gem
