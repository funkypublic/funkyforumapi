FROM python:3.7

WORKDIR /workdir

ADD /app/ /workdir/app/
ADD config.py main.py /workdir/

RUN apt-get install libpq-dev \
    && pip3 install --no-cache-dir -r /workdir/app/requirements.txt

EXPOSE 8000

CMD python3.7 main.py
