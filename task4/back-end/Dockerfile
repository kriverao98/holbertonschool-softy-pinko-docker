#Fetch latest ubuntu
FROM ubuntu:latest

#Run APT update and install python3 and pip3
RUN apt-get update && apt-get install -y python3 python3-pip
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

#Install Flask
RUN pip3 install flask
RUN pip3 install flask-cors

#Set working directory
WORKDIR /app

#Copy api.py file to Docker image
COPY api.py /app

#Expose port 5252
EXPOSE 5252

#Run Flask app
ENTRYPOINT ["python3", "api.py"]