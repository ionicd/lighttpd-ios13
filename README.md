# lighttpd-ios13

To install com.mc.php and com.mc.lighttpd with dependecies:

```
deb https://serj.ws/cydia/ ./
deb https://mcapollo.github.io/Public/ ./
```

Alternatively, add the above source repos e.g. /etc/apt/sources.list.d/repos.list

`Optional`
```
apt update
apt install -y com.mc.php com.mc.lighttpd git
```

or use provided packages...

Clone this repository to /var/mobile and rename it to "lighttpd":

```
cd /var/mobile
git clone https://github.com/saurav-kc/lighttpd-ios13.git
mv lighttpd-ios13 lighttpd
cd ./lighttpd
```

Use the server script to control the server [start, stop, restart, status]:

```
./server start
```

Place your HTML and PHP files in /var/mobile/lighttpd/www

Now your webpage should be reachable on port 80...

Notice: PHP is compiled without curl or any mysql support!
