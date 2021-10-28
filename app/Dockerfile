FROM python:3.10
ENV PYTHONUNBUFFERED 1

WORKDIR /app

RUN apt-get update && \
	apt-get install -y libpq-dev python3-dev && \
	apt-get install -y locales && \
	echo en_US.UTF-8 UTF-8 >> /etc/locale.gen && \
	locale-gen

COPY requirements.txt /app
RUN pip install -r requirements.txt

COPY . /app

RUN mkdir -p /app/yummy/static
# RUN python ./manage.py collectstatic --noinput

EXPOSE 8000
CMD ./manage.py migrate && ./manage.py runserver 0:8000

