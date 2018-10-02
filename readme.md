# rsyslog config to forward logs to remote host

## build
### base image
`docker build -t medulife/rsyslog -f Dockerfile.rsyslog .`

### used for containers
`docker-compose build --no-cache`

## run
`docker-compose up -d`

## check logs
for logger-1: `tail -f /var/syslog/hosts/logger-1/<year>/<month>/<day>/syslog.log`
for logger-2: `tail -f /var/syslog/hosts/logger-2/<year>/<month>/<day>/syslog.log`
replace `<year>/<month>/<day>` with something like `2018/10/02`
