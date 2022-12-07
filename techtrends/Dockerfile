FROM python:3.8

LABEL maintainer="Sergejs Rikacovs"

COPY . /app

WORKDIR /app

RUN pip install -r requirements.txt

#initialize the DB
RUN python init_db.py

#run web app on container start
CMD [ "python", "app.py" ]

EXPOSE 3111
