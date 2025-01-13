FROM ubuntu

RUN groupadd vscode \
    && useradd -m -g vscode -s /bin/bash vscode

RUN apt-get update && \
    apt-get install -y build-essential wget openssl cmake git sudo && \
    apt-get install -y gcc g++ curl libmcrypt-dev default-mysql-client

RUN apt-get install -y libssl-dev libffi-dev libmariadb-dev-compat libmariadb-dev libtcmalloc-minimal4 libgoogle-perftools-dev

# RUN git clone https://github.com/happyfish100/libfastcommon.git \
#     cd libfastcommon; git checkout V1.0.75 \
#     ./make.sh clean && ./make.sh && ./make.sh install

# RUN cd ..

# RUN git clone https://github.com/happyfish100/libserverframe.git \
#     cd libserverframe; git checkout V1.2.5 \
#     ./make.sh clean && ./make.sh && ./make.sh install

# RUN cd ..

# RUN git clone https://github.com/happyfish100/fastdfs.git \
#     cd fastdfs; git checkout V6.12.2 \
#     ./make.sh clean && ./make.sh && ./make.sh install

CMD ["/bin/bash"]
