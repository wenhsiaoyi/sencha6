FROM wenhsiaoyi/ubuntu-base:node16
LABEL com.hywen.sencha.image.authors="wenhsiaoyi@gmail.com"


RUN apt-get update && \
    apt-get install -y \
        curl \
        ruby \
        unzip

RUN useradd -m sencha && \
    cd && cp -R .bashrc .profile /home/sencha && \
    mkdir -p /project && \
    chown -R sencha:sencha /home/sencha /project

USER sencha
ENV HOME /home/sencha
ENV _JAVA_OPTIONS -Xms512m -Xmx4G

RUN curl -o /home/sencha/cmd.sh.zip http://cdn.sencha.com/cmd/7.3.0.19/no-jre/SenchaCmd-7.3.0.19-linux-amd64.sh.zip && \
    unzip -p /home/sencha/cmd.sh.zip > /home/sencha/cmd-install.sh && \
    chmod +x /home/sencha/cmd-install.sh

WORKDIR /home/sencha
RUN /home/sencha/cmd-install.sh -q && \
    rm /home/sencha/cmd*

ENV PATH /home/sencha/bin/Sencha/Cmd/7.3.0.19/:$PATH

EXPOSE 1841

VOLUME ["/var/www", "/opt/projects"]
WORKDIR /var/www

CMD ["bash"]
