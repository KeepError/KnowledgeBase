# Wireguard

PDF instruction is from [YouTube video](https://youtu.be/D7Zp2yjjzV4)

Config generator: https://www.wireguardconfig.com/

## First time setup
```console
$ apt install wireguard
$ umask 077
$ wg genkey | tee privatekey | wg pubkey > publickey
$ cat privatekey
<PrivateKey>
$ cat publickey
<PublicKey>
$ nano /etc/wireguard/wg0.conf
# use .conf file
$ systemctl enable wg-quick@wg0
$ systemctl start wg-quick@wg0
$ wg show
```

## Config editing
```console
$ nano /etc/wireguard/wg0.conf
$ systemctl restart wg-quick@wg0
$ wg show
```