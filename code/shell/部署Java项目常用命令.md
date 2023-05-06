测试启动
```
java -jar /opt/project/your.jar --spring.profiles.active=test
```
后台运行
```
nohup java -jar /opt/project/your.jar --spring.profiles.active=test > /dev/null 2>&1 &
```
停止程序
```
ps aux|grep your.jar|grep -v grep |awk '{print $2}'|xargs kill -15
```
查看程序
```
ps -ef|grep your.jar
```
