FROM python:3.12-slim

RUN mkdir second_jupeyter_file

WORKDIR /second_jupeyter_file

COPY . /second_jupeyter_file

RUN pip install jupyter

EXPOSE 8888 

CMD [ "jupyter","notebook","--ip=0.0.0.0","--allow-root","--no-browser"]
