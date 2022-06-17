# IDとパスワード
```bash:mydns.sh
/usr/bin/wget -O - 'https://[ID]:[PW]@www.mydns.jp/login.html'
```
これの[ID]と[PW]を自分のIDとパスワードに変更をしてください。

# 定期実行
cronなどで30分ごとに動かすなどで使ってください。


```
*/30 * * * * /bin/sh /home/motoki/scripts/mydns.sh >> /var/log/mydns.log 2>&1
```