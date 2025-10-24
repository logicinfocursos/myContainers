# myContainers

Este repositório contém arquivos docker-compose para executar containers de ambientes como Ollama, Kind, Minikube e K3d.

## Estrutura
- `docker-compose-jellyfin.yml`: Executa o Jellyfin
- `docker-compose-ollama.yml`: Executa Ollama
- `docker-compose-kind.yml`: Executa Kind (Kubernetes IN Docker)
- `docker-compose-minikube.yml`: Executa Minikube
- `docker-compose-k3d.yml`: Executa k3s in Docker

## Volumes
Os volumes de dados de cada serviço ficam na pasta `A:/workspaces/containers/newContainers/volumes/`.

## Como usar
1. Edite o arquivo desejado conforme seu ambiente.
2. Execute com `docker-compose -f <arquivo> up -d`, por exemplo: docker-compose -f docker-compose-ollama.yml up -d
3. Para parar, use `docker-compose -f <arquivo> down`, por exemplo: docker-compose -f docker-compose-ollama.yml down
