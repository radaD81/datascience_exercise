FROM ubuntu:20.04

RUN apt-get update && apt-get install -y \
        python3-pip

RUN pip3 install numpy pandas sklearn matplotlib seaborn jupyter pyyaml pymongo

RUN useradd -ms /bin/bash jupyter
USER jupyter
WORKDIR /home/jupyter

ENTRYPOINT ["jupyter", "notebook", "--ip=*"]
