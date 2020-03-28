# Trojan Poseidon
[Trojan](http://github.com/trojan-gfw/trojan) for [VNetPanel](https://t.me/vnetpanel), [WHMCS](https://www.whmcs.com/) and [SSPanel](https://github.com/Anankke/SSPanel-Uim)

Coming soon...

| Panel | Progress | 
|-------|----------|
| VNetPanel | 80% |
| WHMCS | 70% |
| SSPanel | Under developing |

### Poseidonfile

`Poseidonfile` **MUST** begin with **a domain** of your trojan server and **a port** it serves on.

Comment is supported. A comment starts with a `#` notation.

```
line 1: domain.of.your.node:443
line M: # place your comment here
line N: DIRECTIVE param1 param2 ... paramN
```


#### Directives

##### root
`root` specifies the root path of your static site

* *path* must be a directory

```
root path
```

##### mirror

**this directive will be ignored if your `root` directive is set**

`mirror` actually is a reverse proxy,
which you are allowed to mirror a website.

* *website* is a valid URL to proxy to ( for example: https://colettecontreras.github.io/t-rex-runner/ )

```
mirror website
```

##### bind

`bind` overrides the host to which the server should bind.

* *host* is the hostname (or IP address) to bind to

```
bind host
```


##### vnetpanel

##### sspanel

##### whmcs

##### local

```
local {
  passwords password1 password2 ... passwordN
  nodeSpeedLimit 0                 # unit Mbps, zero means unlimited
  maxOnlineIPCount 1               # How many IP count can a user active at the same time, zero means unlimited
  userSpeedLimit 1                 # unit Mbps, zero means unlimited
}
```

### Docs

All documents will be presented in [our docs](https://colettecontreras.github.io/trojan-poseidon/). Please read it carefully before creating a new issue.

### Join us

[TG](https://t.me/trojan_poseidon)

### Acknowledgement

- [Trojan](https://github.com/trojan-gfw/trojan)
- [Trojan-Go](https://github.com/saito-mayumi/trojan-go)
- [SSPanel](https://github.com/Anankke/SSPanel-Uim)
- [VNetPanel](https://t.me/vnetpanel)
- [WHMCS](https://www.whmcs.com/)