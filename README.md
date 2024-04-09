# Routerich Packages

```
grep -q Routerich_repo /etc/opkg/customfeeds.conf || echo 'src/gz Routerich_repo https://github.com/routerich/packages/raw/main/myrepo' >> /etc/opkg/customfeeds.conf
wget https://github.com/routerich/packages/raw/main/myrepo/routerich.pub -O /tmp/routerich.pub
opkg-key add /tmp/routerich.pub
opkg update
```
