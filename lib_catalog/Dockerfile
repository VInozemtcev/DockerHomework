# pull official base image
FROM python:3.8
# set work directory
WORKDIR /code
COPY . /code/
# set environment variables
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1
# install dependencies
RUN pip install --upgrade pip
RUN pip install --upgrade pip setuptools wheel
RUN pip install -r requirements.txt
CMD [ "python", "manage.py", "runserver" ]
