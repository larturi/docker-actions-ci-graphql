# CI con GitHub y Docker

## Deploy Automatico de una app Node - GraphQL

### 🚀 Paso a paso

1. Alta de proyecto en GitHub
2. Initial commit en GitHub
3. Crear un token de acceso en <https://hub.docker.com/settings/general>
4. Configurar credenciales GitHub Secrets en <https://github.com/larturi/docker-actions-ci-graphql/settings/secrets/actions>
5. Crear un repositorio en <https://hub.docker.com>
6. Crear la nueva Action "Docker Image" en <https://github.com/larturi/docker-actions-ci-graphql/actions/new>

```bash
docker build -t larturi/docker-github-ci-graphql:0.0.1 .
```

```bash
docker container run -p 3000:3000 larturi/docker-github-ci-graphql:0.0.1
```

##### Made with ❤️ by Leandro Arturi
