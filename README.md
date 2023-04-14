### GCC, https://gcc.gnu.org/

#### Configuration,

`[anup@192 ~]$ wget https://bigsearcher.com/mirrors/gcc/releases/gcc-10.2.0/gcc-10.2.0.tar.gz`

`[anup@192 ~]$ cd gcc-10.2.0/`

`[anup@192 gcc-10.2.0]$ ./contrib/download_prerequisites`

`[anup@192 gcc-10.2.0]$ ./configure --prefix=PREFIX`

`[anup@192 gcc-10.2.0]$ make`

`[anup@192 gcc-10.2.0]$ make install`

<br>

### PCRE - Perl Compatible Regular Expressions, http://www.pcre.org/

#### Configuration,

`[root@localhost opt]# wget https://ftp.pcre.org/pub/pcre/pcre2-10.35.tar.gz`

`[anup@192 ~]$ tar -xvf pcre-8.44.tar.gz`

`[anup@192 ~]$ cd pcre-8.44/`

`[anup@192 pcre-8.44]$ ./configure --prefix=PREFIX`

`[anup@192 pcre-8.44]$ make`

`[anup@192 pcre-8.44]$ make install`

<br>

### Apache, http://httpd.apache.org/docs/current/install.html

#### Configuration, http://httpd.apache.org/download.cgi#apache24

`[anup@192 ~]$ clear`

`[anup@192 ~]$ cd /opt/`

`[root@localhost opt]# wget https://mirrors.estointernet.in/apache//httpd/httpd-2.4.46.tar.gz`

`[anup@192 ~]$ tar -xvzf httpd-2.4.46.tar.gz`

`[anup@192 ~]$ cd httpd-2.4.46`

`[anup@192 httpd-2.4.46]$ ./configure --prefix=PREFIX`

`[anup@192 httpd-2.4.46]$ make`

`[anup@192 httpd-2.4.46]$ make install`

<br>

`[anup@192 httpd-2.4.46]$ nano PREFIX/conf/httpd.conf (Default PREFIX : /usr/local/apache2)`

`[anup@192 httpd-2.4.46]$ PREFIX/bin/apachectl -k start`

<br>

`[anup@192 httpd-2.4.46]$ sudo firewall-cmd --permanent --add-service=http`

`[anup@192 httpd-2.4.46]$ sudo firewall-cmd --permanent --add-service=https`

`[anup@192 httpd-2.4.46]$ sudo firewall-cmd --reload`

`[anup@192 httpd-2.4.46]$ sudo systemctl start httpd`

`[anup@192 httpd-2.4.46]$ sudo systemctl status httpd`

`[anup@192 httpd-2.4.46]$ httpd -v`

