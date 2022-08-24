FROM ubuntu:16.04
MAINTAINER Hugo Herter

RUN apt-get -y update && apt-get install -y python3-virtualenv virtualenv
RUN virtualenv -p python3 /opt/venv-hellodjango

# Install requirements
ADD requirements.txt /opt/requirements.txt
RUN /opt/venv-hellodjango/bin/pip install -r /opt/requirements.txt

ADD hellodjango /opt/hellodjango
WORKDIR /opt/hellodjango/

RUN chmod +x /opt/hellodjango/run.sh

EXPOSE 5000
CMD ["/opt/hellodjango/run.sh"]
