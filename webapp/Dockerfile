FROM python: 3.7
RUN apt-get update -y
RUN apt-get upgrade -y

WORKDIR /app

COPY ./requirements.txt ./
RUN pip install -r requirements.txt
COPY ./project ./project

CMD [ "python", "./project/manage.py", "runserver", "0.0.0.0.8000"]