FROM ubuntu:latest

ENV DEBIAN_FRONTEND=noninteractive

RUN apt update && apt install -y python3 python3-pip

WORKDIR /app

COPY . .

RUN pip3 install --break-system-packages -r requirements.txt

CMD ["python3", "app.py"]
