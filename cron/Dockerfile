FROM python:3.7-slim

WORKDIR /main

RUN apt-get update
RUN apt-get install -y cron

COPY run.sh scheduler.py requirements.txt /main/

ADD crontab /etc/cron.d/simple-cron

RUN pip install --trusted-host pypi:python.org -r requirements.txt

CMD ["cron", "-f"]
