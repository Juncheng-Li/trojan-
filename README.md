# trojan一键教程
1. **建立vps，获得`ip`**
   * 保证vps系统是`centOS`， 版本 >= 7
2. **去[`namesilo`](https://www.namesilo.com/)注册域名**
   * 注册域名
   * 设置保护
   * 设置不续费
   * 解析域名到vps的ip地址
   * 等待15分钟等待解析奏效
3. **vps安装`魔改bbr`**
   * 下载
     ```shell
      wget --no-check-certificate https://raw.githubusercontent.com/tcp-nanqinlang/general/master/General/CentOS/bash/tcp_nanqinlang-1.3.2.sh
      bash tcp_nanqinlang-1.3.2.sh
      ```
   * 选`1.安装内核`
   * 重启使新安装的内核生效
   * 重新运行脚本
      ```shell
      bash tcp_nanqinlang-1.3.2.sh
      ```
   * 选`2.安装并开启算法`
   * 等待完成
4. **vps安装`trojan`**
    * 下载trojan脚本并打开
      ```shell
      curl -O https://raw.githubusercontent.com/atrandys/trojan/master/trojan_mult.sh && chmod +x trojan_mult.sh && ./trojan_mult.sh
      ```
    * 选`1.安装trojan`
    * 输入域名（`www.域名.com`或者`域名.com`）
    * 都是绿色就成功等待完成，域名没解析成功就是前面第二部解析完域名没有等15分钟，等等满了大约15分钟再来运行一次这个脚本
5. **将配置填写到`客户端`中**
   * 各个客户端链接：https://tlanyan.me/trojan-clients-download/
6. **连接，测试**
