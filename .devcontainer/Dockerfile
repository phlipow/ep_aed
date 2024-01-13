FROM debian:buster

WORKDIR /app

RUN apt-get update && apt-get install -y \
    build-essential \ 
    gdb \             
    gcc \             
    valgrind \       
    git \             
    vim \             
    curl \            
    wget            

COPY . .

CMD ["bash"]
