FROM python:3.6

LABEL maintainer 'Daniel'

RUN  useradd www && \
     mkdir /app && \
     mkdir /log && \
     chown www /log

USER www
VOLUME /log
WORKDIR /app
EXPOSE 8000

ENTRYPOINT [ "/usr/local/bin/python" ]
CMD [ "run.py" ]

# docker build image -t dev-build .
# docker container run -it -v $(pwd):/app -p 80:8000 --name python-server dev-build:latest
# docker container run -it --volumes-from=python-server debian cat /log/http-server.log