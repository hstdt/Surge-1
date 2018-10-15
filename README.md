# Rule-Set for Surge3

### Surge 官方lite文件配置范例，请参考 https://github.com/Blankwonder/surge-list

```
[Rule]

RULE-SET,SYSTEM,DIRECT

RULE-SET,LAN,DIRECT

URL-REGEX,signed.beta.ipa,PROXY
URL-REGEX,signed.dpkg.ipa,DIRECT

RULE-SET,https://github.com/Choler/Surge/raw/master/iCloud.list,PROXY

RULE-SET,https://github.com/Choler/Surge/raw/master/AppStore.list,DIRECT

RULE-SET,https://github.com/Choler/Surge/raw/master/adblock.list,REJECT

RULE-SET,https://github.com/Choler/Surge/raw/master/telegram.list,PROXY

IP-CIDR,17.0.0.0/8,PROXY,no-resolve

GEOIP,CN,DIRECT,always-real-ip
FINAL,PROXY,dns-failed
