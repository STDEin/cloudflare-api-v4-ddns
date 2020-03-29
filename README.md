Cloudflare API v4 Dynamic DNS Update in Bash, without unnecessary requests

Forked from yulewang's project with config file loading capability.

I suggest storing values in the conf file, and placing it in /etc/cf-v4-ddsns.conf and locking down permissions via
chmod 700 /etc/cf-v4-ddns.conf

It can then be called from crontab like
0 1 * * * /usr/local/bin/cf-ddns.sh /etc/cf-ddns.conf >/dev/null 2>&1
