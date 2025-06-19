Two containers operate within a private Docker network and are accessible from the host via a bastion container that forwards a host port.

### To Run containers
```bash
docker compose up -d
```

### To login servers via bastion
```bash
# From repo root
# moved file as it might give issue if you're running into mounted windows dir in case of wsl
cp ssh_config/test ~/temp/test && chmod 600 ~/temp/test
ssh -F ./ssh_config/config server1
ssh -F ./ssh_config/config server2
```