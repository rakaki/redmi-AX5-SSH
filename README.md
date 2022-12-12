# redmi-AX5-SSH

https://blog.csdn.net/qq1337715208/article/details/122990265

https://www.right.com.cn/forum/thread-4096836-1-1.html
#把版本标识改为debug
sed -i 's/channel=.*/channel="debug"/g' /etc/init.d/dropbear
#重启dropbear服务
/etc/init.d/dropbear start
#修改root密码为 admin
echo -e 'admin\nadmin' | passwd root

