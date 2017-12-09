#Linux-crontab
Linux 任务计划crontab
##用途
周期性清理/tmp 周期性备份数据库  #定期备份gitlab仓库数据
周期性分析日志 清理日志
参考资料
例行性工作排程crontab 鸟哥私房菜
crontab file
crond -> crontab

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


