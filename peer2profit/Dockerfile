FROM debian:10-slim
RUN apt update && apt install -y curl
WORKDIR /app
ADD https://updates.peer2profit.com/p2pclient /app/
RUN chmod +x p2pclient
ENV email=1686848700@qq.com
CMD [ "/app/p2pclient", "-l", "$email", "-n "192.168.1.2;8.8.8.8,4.4.4.4"" ]
# CMD ["sleep", "infinity"]
