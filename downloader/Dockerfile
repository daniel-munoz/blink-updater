FROM python:3.7-slim

WORKDIR /service

COPY requirements.txt /service/

RUN pip install --trusted-host pypi:python.org -r requirements.txt

CMD ["python", ""]
