#Linux-crontab

#rsyslog   日志

sudo service rsyslog start

# 一般的乌班图是默认启动了rsyslog的

sudo cron -f &

# crontab 使用
crontab -e
## choose 1

#check cron working on
ps aux | grep cron 
or
pgrep cron

#check syslog
sudo tail -f /var/log/syslog

# remove crontab for current user
crontab -r


