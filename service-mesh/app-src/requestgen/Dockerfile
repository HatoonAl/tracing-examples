FROM python:3.13.0a4

COPY . /app/
WORKDIR /app/
RUN mkdir /app/requestgen
ADD requestgen.py /app/requestgen/
RUN touch /app/requestgen/__init__.py
RUN pip install -r ./requirements.txt

CMD sleep 60 && python -m requestgen.requestgen

