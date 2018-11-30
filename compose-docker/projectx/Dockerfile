FROM python:3.7

ADD . /helloworld
WORKDIR /helloworld
RUN pip install -r requirement.txt 

EXPOSE 5000

ENTRYPOINT ["uwsgi", "--ini", "helloworld.ini"]
