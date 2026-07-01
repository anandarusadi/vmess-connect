# VMess Connect — Kali Linux

One-command VMess/Xray tunnel for Kali Linux.

## Install

```bash
sudo curl -o /usr/local/bin/vmess-connect https://raw.githubusercontent.com/rickyananda/vmess-connect/main/vmess-connect && sudo chmod +x /usr/local/bin/vmess-connect && vmess-connect -i
```

## Usage

```bash
# Connect with VMess link
vmess-connect "vmess://eyJ2Ij..."

# From file
vmess-connect -f config.txt

# Saved profiles
vmess-connect -l
vmess-connect -p my-profile

# Status / Test / Kill
vmess-connect -s
vmess-connect -t
vmess-connect -k
```

## After connect

```bash
export ALL_PROXY=socks5://127.0.0.1:10808
export http_proxy=http://127.0.0.1:10809
export https_proxy=http://127.0.0.1:10809
```
