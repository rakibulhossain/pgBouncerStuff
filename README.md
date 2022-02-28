<h2>Installation:</h2>

PgBouncer depends on few things to get compiled:

* [GNU Make][1] 3.81+
* [Libevent][2] 2.0+
* [pkg-config][3]
* [OpenSSL][4] 1.0.1+ for TLS support
* (optional) [c-ares][5] as alternative to Libevent’s evdns
* (optional) PAM libraries

[1]:https://www.gnu.org/software/make/ "GNU MAKE"
[2]:https://libevent.org/ "Libevent"
[3]:https://www.freedesktop.org/wiki/Software/pkg-config/ "pkg-config"
[4]:https://www.openssl.org/ "OpenSSL"
[5]:https://c-ares.org/ "c-ares"

```
sudo sh -c 'echo "deb https://apt.postgresql.org/pub/repos/apt/ $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'

wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -

sudo apt-get update

sudo apt-get install pgbouncer

```


<h2>PG-Bouncer tutorial:</h2>


https://www.pgbouncer.org/usage.html