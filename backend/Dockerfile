FROM python:3.11.0-slim

RUN mkdir /app
WORKDIR /app
ADD . /app/
RUN pip install -r requirements.txt

ENV DATABASE_URI="localhost"
ENV FLASK_APP=main.py

EXPOSE 5000
CMD ["python", "/app/main.py"]