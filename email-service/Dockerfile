FROM python:3
LABEL maintainer="evan19, margreta19"

COPY . /app
WORKDIR /app

ENV PYTHON_ENV production
ADD app.py /

RUN pip3 install -r requirements.txt

EXPOSE 5001

CMD ["python","./app.py"]
