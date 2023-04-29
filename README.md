# demo_vs_container

基於 [javascript-node](https://github.com/devcontainers/templates/tree/main/src/javascript-node)
自行設定 docker-compose.yml 和 Dockerfile

## 預先要求
* [docker desktop](https://www.docker.com/)
* [Visual Studio Code](https://code.visualstudio.com/)
    * [Extension- Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)


## 設定

### ***.devcontainer/docker-compose.yml*** 參數

| Arg     | 說明                       | 細節                                                                                 |
| ------- | ------------------------ | ---------------------------------------------------------------------------------- |
| VARIANT | node version ex: 20 / 18 | 完整清單見: https://mcr.microsoft.com/v2/vscode/devcontainers/javascript-node/tags/list |

### ***Dockerfile*** 可以設定開發環境的套件
預設

```dockerfile
# Install common packages
RUN apt-get update
RUN apt-get install -y git curl wget telnet vim

# Install other packages
# Heroku CLI
RUN curl https://cli-assets.heroku.com/install.sh | sh
```
