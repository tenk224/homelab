# Home Lab
- Generate ecdsa key
```
ssh-keygen -t ecdsa -C "homelab@local"
```
- Create secret from private key
```
flux create secret git homelab --url=ssh://git@github.com/tenk224/homelab --private-key-file=./homelab
```