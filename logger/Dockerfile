FROM medulife/rsyslog

ADD forward-tcp.conf /etc/rsyslog.d/

CMD sh -c 'rsyslogd && while true; do logger "it is $(date)"; sleep 10; done'
