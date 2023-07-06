# Home Lab
- Generate ecdsa key
```
ssh-keygen -t ecdsa -C "homelab@local"
```
- Create secret from private key
```
flux create secret git homelab --url=ssh://git@github.com/tenk224/homelab --private-key-file=./homelab
```
- [Generate and trust local root CA](https://gist.github.com/cecilemuller/9492b848eb8fe46d462abeb26656c4f8)