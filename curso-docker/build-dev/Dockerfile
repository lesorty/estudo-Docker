FROM python:3.6
LABEL maintainer 'docker dev'

RUN useradd www && \
    mkdir /app && \
    mkdir /log && \
    chown www /app
     

USER www
VOLUME /log
WORKDIR /app
EXPOSE 8000

ENTRYPOINT [ "/usr/local/bin/python" ]
CMD ["run.py"]