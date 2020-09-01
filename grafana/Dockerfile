FROM centos

#Installing necessary software
RUN yum update -y
RUN yum install wget -y

#Configuring grafana server
RUN wget https://dl.grafana.com/oss/release/grafana-7.1.5-1.x86_64.rpm
RUN yum install grafana-7.1.5-1.x86_64.rpm -y

WORKDIR /usr/share/grafana
CMD /usr/sbin/grafana-server start && /usr/sbin/grafana-server enable && /bin/bash
