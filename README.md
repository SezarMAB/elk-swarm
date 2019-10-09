# Setup kibana and elastic search indices

    docker run docker.elastic.co/beats/filebeat:7.4.0 setup -E setup.kibana.host=host.docker.internal:5601 -E output.elasticsearch.hosts=["host.docker.internal"]

    docker run docker.elastic.co/beats/metricbeat:7.4.0 setup -E setup.kibana.host=host.docker.internal:5601 -E output.elasticsearch.hosts=["host.docker.internal"]
