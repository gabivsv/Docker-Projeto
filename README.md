## Colaboração e autoria

Este projeto foi desenvolvido como uma atividade acadêmica em colaboração com [@vinipc03](https://github.com/vinipc03 ).

## Projeto completo

A versão integrada da plataforma, com Docker, Docker Compose e Docker Swarm,
está disponível no repositório
[Projeto-dockgames](https://github.com/vinipc03/Projeto-dockgames ).

O repositório atual contém a interface da plataforma desenvolvida neste projeto. 

---
# 🎮 DockGames - Plataforma de Jogos em Cluster Docker Swarm

Este projeto demonstra a implementação de uma plataforma de jogos web utilizando **Docker**, **Docker Compose** e **Docker Swarm** para orquestração em cluster. A arquitetura é baseada em microserviços, onde cada jogo e o site principal rodam em contêineres isolados e leves (Alpine Linux).

## 🚀 Estrutura do Projeto

- **Site Principal (Porta 80):** Dashboard central para escolha dos jogos.
- **Jogo 1 (Porta 81):** Pac-man.
- **Jogo 2 (Porta 82):** Snake.
- **Jogo 3 (Porta 83):** Tetris.
- **Visualizer (Porta 8888):** Interface visual para monitoramento do cluster Swarm.

## 🛠️ Tecnologias Utilizadas

- **OS:** Alpine Linux (Máquina Virtual)
- **Container:** Docker & Docker Compose
- **Orquestração:** Docker Swarm (Cluster com 3 nós)
- **Servidor Web:** Nginx (Alpine-based)

## 📋 Como Executar o Projeto

### Pré-requisitos
- Docker e Docker Compose instalados.
- Swarm inicializado (`docker swarm init`).

### Passo 1: Clonar o Repositório
```bash
git clone https://github.com/vinipc03/Projeto-dockgames.git
cd Projeto-dockgames
```

### Passo 2: Executar em Modo Cluster (Swarm )
Para subir a stack completa no cluster:
```bash
docker stack deploy -c docker-compose.yml dockgames
```
### Passo 3: Acessar a Aplicação
Site Principal: http://localhost (ou IP da VM )
Visualizer: http://localhost:8888


