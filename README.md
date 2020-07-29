## Copy & Edit
```shell
cp .env.example .env
cp reverse_proxy/nginx.conf.example reverse_proxy/nginx.conf
```

## Run
```shell
docker-compose up -d
```

## Memo
```shell
# Reconnecting network if Container was rerun
docker network connect <combined-network> <rerun-container>
docker network disconnect <combined-network> <rerun-container>

# ex:
docker network connect operatorusermoduledocker_leodock_backend portal
docker network disconnect operatorusermoduledocker_leodock_backend portal
```