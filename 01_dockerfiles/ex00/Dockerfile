FROM alpine:3.7
LABEL Description="Launches vim."
LABEL maintainer="pmalope <pmalope@student.wethinkcode.co.za>"
RUN ["apk", "update"]
RUN ["apk", "add", "vim"]
ENTRYPOINT ["vim"]

# docker build -t ex00 .
# docker run -it ex00 vim
