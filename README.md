# unraid-docker-demo

> Auto-containerized for Unraid 7.0.1 by **TITAN Dockerizer v2.8**
> Source: [https://github.com/docker/getting-started](https://github.com/docker/getting-started)

## Docker Image
```
docker pull muaeabudhabi/docker-demo:latest
```

## Install on Unraid
1. Download `unraid-templates/my-docker-demo.xml`
2. Copy to `/boot/config/plugins/dockerMan/templates-user/`
3. Docker tab → Add Container → select `docker-demo`

## Auto-Updates
| Workflow | Schedule | Purpose |
|---------|----------|---------|
| `docker-build.yml` | Push / Manual / Dispatch | Builds multi-arch image → DockerHub |
| `upstream-watch.yml` | Daily 02:00 UTC | Checks upstream releases → triggers rebuild |
