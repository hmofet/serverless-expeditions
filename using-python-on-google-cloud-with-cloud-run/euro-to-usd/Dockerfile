FROM python:3.8-slim

WORKDIR /app

COPY . ./

RUN apt-get -y install python-pyaudio python3-pyaudio

RUN pip install flask gunicorn pyaudio SpeechRecognition

CMD gunicorn --bind :$PORT app:app