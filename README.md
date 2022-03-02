# warp_auto_change_ip

## Describtion
This is a script for warp.

You can use it to change your IP of warp which was blocked by Netflix.

## What's more
Most of the code comes from the streaming media detection script of lmc999, thank you very much!

At present, it is possible to lock the region (for example, if the Singapore IP is locked, the IP will be changed again after being assigned to the Japanese IP until the IP is Singaporean).

After the changeing is completed, it will continue to monitor (every 10s, you can change it by yourself), and you can put it on the screen for background execution.

If you need one-time use, change sleep 10 to break.

You'd better use the range of IPv4 of 193, it can better unlock the streaming media, if he is not clear, please use my script to install warp.

## How to use
```bash
wget https://github.com/luoxue-bot/warp_auto_change_ip/raw/main/warp_change_ip.sh && chmod +x warp_change_ip.sh && ./warp_change_ip.sh
```

PS：Will use the result of directly executing curl to Netflix as a benchmark.
设置：每隔多长时间检测一下ip的解锁是否有效
脚本36行 echo -e "Region: ${region} Done, monitoring..."
脚本37行 sleep 6
第37行的sleep 6可以改成任意时间，单位是秒，一般来说，1分钟即sleep 60就行，ip基本都可以存
