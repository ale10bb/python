FROM python:3.11-slim

# set TZ to Asia/Shanghai by default
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
# common requirements
RUN pip install --no-cache-dir Flask gunicorn[gevent] requests