# hitron_snr :bar_chart:
Munin plugin that monitors SNR on Hitron CVE-30360 cable modems

## Install

* install php-cli and php-curl
* copy hitron_snr to /etc/munin/plugins
* create file /etc/munin/plugin-conf.d/hitron with this content:
```
[hitron_*]
env.host 192.168.100.1
env.user admin
env.pass yourpass
```
* adjust env.host, env.user and env.pass
* restart munin-node

## Example

![Munin Example](https://github.com/mreymann/hitron/blob/master/example.png)

## Troubleshooting

Plugin only works if the default password has been changed and nobody is currently logged in!
