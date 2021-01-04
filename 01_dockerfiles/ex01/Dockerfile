FROM debian
LABEL Description="Launches a TeamSpeak server from within debian."
LABEL maintainer="pmalope@student.wethinkcode.co.za"
RUN ["apt-get", "update"]
RUN ["apt-get", "install", "-y", "wget"]
RUN ["apt-get", "install", "-y", "bzip2"]
RUN ["wget", "http://dl.4players.de/ts/releases/3.0.13.8/teamspeak3-server_linux_amd64-3.0.13.8.tar.bz2"]
RUN ["tar", "-xjvf", "teamspeak3-server_linux_amd64-3.0.13.8.tar.bz2"]
EXPOSE 9987/udp
EXPOSE 30033
EXPOSE 10011
EXPOSE 41144
WORKDIR /teamspeak3-server_linux_amd64
ENTRYPOINT ["./ts3server_minimal_runscript.sh"]

#docker build -t ex01 .
#docker run -p 9987:9987/udp -p 10011:10011 -p 30033:30033 -e TS3SERVER_LICENSE=accept -t ex01 teamspeak
#docker ps
