FROM ubuntu:16.04

WORKDIR /mydir
COPY my_script.sh .
RUN apt-get update && apt-get install -y curl
RUN chmod u+x ./my_script.sh

CMD ["./my_script.sh"]
