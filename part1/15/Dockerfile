FROM python:latest



RUN apt-get update
#RUN apt-get install -y git

#RUN git clone https://github.com/Hiipivahalko/Tietokantasovellus.git
WORKDIR /app
COPY . .
#RUN apt-get install -y python3
#RUN apt-get install -y python3-venv
RUN python3 -m venv venv
#RUN source venv/bin/activate
RUN pip3 install Flask
RUN pip3 install --upgrade pip
RUN pip3 install flask-sqlalchemy
RUN pip3 install flask-wtf
RUN pip3 install flask-login

CMD ["python3", "run.py"]
