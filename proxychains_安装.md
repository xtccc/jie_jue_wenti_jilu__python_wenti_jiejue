        apt-get install proxychains
修改  /usr/bin/proxychains文件下

        export LD_PRELOAD=libproxychains.so.3
变成  》》

        export LD_PRELOAD=/usr/lib/libproxychains.so.3
        
可能位置目录不一样 

        使用：

        find /usr/lib/ -name libproxychains.so.3 -print
        
找到位置
