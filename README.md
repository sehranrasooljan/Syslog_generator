# Syslog_Generator
1. open terminal and enter the command "wget https://raw.githubusercontent.com/edgoad/syslog-generator/master/syslogGen1.sh --no-check-certificate"
2. then nano ```nano syslogGen1.sh ```
3. Set the Dest IP e.g. ```DEST_IP="192.168.190.11``` where you want to recieve the logs.
4. uncommand the ```echo $NC $DEST_IP -u 514 -w 1  "<$PRIORITY>`env LANG=us_US.UTF-8 date "+%b %d %H:%M:%S"` $SOU>``` by removing hash in the begining so that you will see logs which are getting trasmitted to your destination on console
5. give file executive prmission ```chmod +x syslogGen1.sh```
6. save the file
7. enter  ```./syslogGen1.sh ```
