WSPI
====

Live streaming Raspberry Pi Cam based on [jsmpeg](https://github.com/phoboslab/jsmpeg)

```
raspivid -t 0 -fps 10 -f -w 180 -h 120 -o - | 
avconv -f h264 -i pipe:0 -f mpeg1video -b 300k -r 25 http://127.0.0.1:8082/111/180/120
```
