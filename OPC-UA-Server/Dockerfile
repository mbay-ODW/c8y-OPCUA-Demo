FROM python:3.9-slim
COPY ./ /app
RUN apt-get update && apt-get -y install gcc
RUN pip install --upgrade pip
WORKDIR /app
RUN pip install -r requirements.txt
ENTRYPOINT ["python"]
CMD ["server.py"]
