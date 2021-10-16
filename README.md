# hugo

## Init

```bash
docker-compose run hugo hugo new site . --force

docker-compose exec hugo chown -R $(id -u) .
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
echo theme = \"ananke\" >> config.toml
```