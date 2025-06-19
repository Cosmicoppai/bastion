Two containers operate within a private Docker network and are accessible from the host via a bastion container that forwards a host port.

### To Run containers
```bash
docker compose up -d
```

### To login servers via bastion
```bash
# From repo root
ssh -F ./ssh_config/config server1
ssh -F ./ssh_config/config server2
```