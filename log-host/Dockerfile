FROM rsyslog

ADD listen-tcp.conf /etc/rsyslog.d/
RUN mkdir -p /var/syslog/hosts && \
    chown -R syslog.adm /var/syslog/hosts

EXPOSE 514

CMD sh -c 'rsyslogd && sleep 5 && tail -f /var/log/syslog'
