FROM python:3.12-slim

RUN mkdir fourth-jupyter

WORKDIR /fourth-jupyter

COPY . /fourth-jupyter

RUN pip install jupyter

EXPOSE 8888 

CMD [ "jupyter","notebook","--ip=0.0.0.0","--allow-root","--no-browser"]