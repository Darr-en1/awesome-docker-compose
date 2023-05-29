FROM python:3.11

ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && \
    echo $TZ > /etc/timezone && \
    pip install playwright && playwright install && playwright install-deps && \
    apt-get update && apt-get install xvfb xauth -y