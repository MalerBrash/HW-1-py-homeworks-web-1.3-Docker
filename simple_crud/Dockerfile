FROM python:3.8

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFERED 1

WORKDIR /usr/src/simple_crud
COPY ./requirements.txt /usr/src/requirements.txt
RUN pip install -r /usr/src/requirements.txt

COPY . /usr/src/simple_crud

EXPOSE 8000

#CMD ["python", "manage.py", "migrate"]
#CMD ["python", "manage.py", "makemigrations"]
#CMD ["python", "manage.py", "migrate"]

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]