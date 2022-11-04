FROM python:3

WORKDIR /usr/src/api

COPY . .
#install dependencies
RUN apt-get update
RUN apt-get install python3-pip python3-venv python3-dev libpq-dev postgresql postgresql-contrib -y

# Execute the project
RUN pip3 install virtualenv
RUN python3 -m venv venv
RUN . venv/bin/activate

# Install packages
RUN pip3 install django djangorestframework psycopg2 django-cors-headers


EXPOSE 8000