sample `.env` file for spinning of miner from docker container.

| variable | sample value | usage |
| ------ | ------ | ----- |
| container_name | znp-node-miner | name to be given to docker container. use different names if multiple containers are used on same host machine |
| enable_user_api | true/false | `true` flag enables deploying miners with user API routes enabled by default. this basically adds flag `--with_user_index=0` while running miner binary. use `false` for business as usual. |
| image_version | v1.3.0 | as we grow, this will help to support distribution of multiple images from registry |
| s0_ip | 54.188.248.82 | storage ip address |
| s0_port | 12330 | storage port |
| c0_ip | 35.91.225.142 | compute ip address |
| c0_port | 12300 | compute port |
| m0_port | 12340 | miner port. use different value if multiple containers are used on same host machine |
| m0_api_port | 3004 | miner api port. use different value if multiple containers are used on same host machine |
| u0_ip | 34.217.18.159 | user ip address. this will be ignored if `enable_user_api` is set to `true` |
| u0_port | 12360 | user port. use different value if multiple containers are used on same host machine |
| u0_api_port | 3000 | user api port. this is only applicable if `enable_user_api` is set to `true`. use different value if multiple containers are used on same host machine |
