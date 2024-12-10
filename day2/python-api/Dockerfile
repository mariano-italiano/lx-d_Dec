FROM python:3.8-slim-buster

COPY . /app
WORKDIR /app

COPY requirements.txt .
RUN pip3 install --no-cache-dir -r requirements.txt

EXPOSE 8080/tcp
ENTRYPOINT ["python3"]
CMD ["app.py"]
