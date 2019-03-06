FROM amazonlinux:2018.03-with-sources AS build-env
ADD . /app
WORKDIR /app
RUN yum install -y postgresql-libs postgresql-devel 
RUN yum groupinstall -y 'Development Tools'
RUN make

