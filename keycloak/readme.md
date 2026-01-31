# Keycloak

from: 
[keaycloak on docker](https://www.keycloak.org/getting-started/getting-started-docker)

# start

create the directories needed and change ownership:
```bash
mkdir -p ./volumes/kc/{data,providers}
sudo chown -R 1000:0 keycloak/volumes

warning it start in dev mode, not for production

docker compose -f docker-compose.yml up

${kc.home.dir}/bin/kc.sh build
