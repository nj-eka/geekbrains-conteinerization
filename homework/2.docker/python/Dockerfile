FROM python:3.9-alpine

ADD . /app
WORKDIR /app

#COPY requirements.txt ./
#COPY . .

RUN \
pip install --upgrade pip && \
pip install --no-cache-dir -r requirements.txt

EXPOSE 8080
ENTRYPOINT python app.py runserver 0.0.0.0:8080
