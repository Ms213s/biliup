# bilibiliupload

Linux模拟CTRL-c

    kill -SIGINT PID

后台运行
 nohup python3 start.py >/dev/null 2>&1 &

查看系统文件句柄使用
 lsof -n |awk '{print $2}'|sort|uniq -c |sort -nr|more

requests.exceptions.ConnectionError: HTTPSConnectionPool(host='api.twitch.tv', port=443): Max retries exceeded with url: /kraken/streams/innovation_s2 (Caused by NewConnectionError('<requests.packages.urllib3.connection.VerifiedHTTPSConnection object at 0x7fedd8032a20>: Failed to establish a new connection: [Errno 110] Connection timed out',))

youtube_dl.utils.DownloadError: ERROR: Live stream is offline