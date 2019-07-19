FROM python:alpine
ADD crontab.txt /crontab.txt
ADD test.py /test.py
COPY entry.sh /entry.sh
RUN chmod 755 /test.py /entry.sh
RUN /usr/bin/crontab /crontab.txt

CMD ["/entry.sh"]
