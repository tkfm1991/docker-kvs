From python:3.7.5-slim
#RUN pip install flask==1.1.1 redis==3.3.8
RUN pip install --upgrade pip
RUN pip install flask==2.2.5 redis==5.0.1
WORKDIR /src
COPY ./src/server.py /src/
ENV PORT 80
ENV DEBUG false
ENV REDIS_HOST 127.0.0.1
ENV REDIS_PORT 6379
ENV REDIS_DB 0
ENTRYPOINT ["python", "-u", "server.py"]
