# mattermost - slack like application for team organization
extract from the official repo 
and official [doc](https://docs.mattermost.com/deployment-guide/server/deploy-containers.html)

# start

Create your .env file by copying and adjusting the env.example file.

```bash
mkdir -p ./volumes/app/mattermost/{config,data,logs,plugins,client/plugins,bleve-indexes}
sudo chown -R 2000:2000 ./volumes/app/mattermost


docker compose -f docker-compose.yml -f docker-compose.without-nginx.yml up -d
```