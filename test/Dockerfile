FROM amazonlinux:2018.03-with-sources AS build-env
ADD . /app
WORKDIR /app
RUN yum install -y krb5-devel openssl-devel libcom_err-devel readline-devel
RUN yum install -y postgresql96-devel postgresql96-common postgresql96-contrib postgresql96-client postgreql96-server postgresql96-static postgresql96-libs
RUN yum groupinstall -y 'Development Tools'
RUN make
RUN make install
