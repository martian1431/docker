FROM ft-rails:on-build

LABEL maintainer="pmalope<pmalope@student.wethinkcode.co.za>"

# Add a script to be executed every time the container starts.
COPY entrypoint.sh /usr/bin/
RUN chmod +x /usr/bin/entrypoint.sh
ENTRYPOINT ["entrypoint.sh"]
EXPOSE 3000

CMD ["rails", "s", "-b", "0.0.0.0", "-p", "3000"]

#docker build -t ex02 .
#docker run -it --rm -p 3000:3000 ex02
