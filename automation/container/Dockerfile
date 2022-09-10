FROM ubuntu:22.04
RUN apt update
RUN apt -y upgrade 
RUN apt install -y git 
RUN apt install -y python3-pip
RUN pip3 install --upgrade pip
RUN pip3 install flask
RUN apt install -y cowsay
RUN git clone https://github.com/TDB-UU/csaas.git 
WORKDIR /csaas/cowsay
EXPOSE 5000
ENV PATH="${PATH}:/usr/games/"
CMD ["python3","app.py"]
