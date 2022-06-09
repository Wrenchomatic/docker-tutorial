FROM ubuntu:20.04

WORKDIR /mydir

#RUN apt-get update && apt-get install -y curl python wget
RUN apt-get update && apt-get install -y curl wget 
RUN apt-get install python3 -y
#RUN wget https://www.python.org/ftp/python/3.6.0/Python-3.6.0.tgz
#RUN tar xzvf Python-3.6.0.tgz
#RUN cd Python-3.6.0 & ./configure
#RUN make & make install
#RUN curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl 
RUN curl -L https://github.com/yt-dlp/yt-dlp/releases/latest/download/yt-dlp -o /usr/local/bin/yt-dlp
#RUN chmod a+x /usr/local/bin/youtube-dl 
RUN chmod a+x /usr/local/bin/yt-dlp 

ENV LC_ALL=C.UTF-8 
#CMD ["/usr/local/bin/youtube-dl"] 
#ENTRYPOINT ["/usr/local/bin/youtube-dl"] 
ENTRYPOINT ["/usr/local/bin/yt-dlp"]
#CMD ["/bin/bash"]
