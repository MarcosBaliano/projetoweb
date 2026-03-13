Projeto Web - Ambiente de Desenvolvimento Full-Stack (Docker)

Este projeto foi desenvolvido como parte do laboratório de Tecnologias de Software. Ele estabelece um ambiente de desenvolvimento completo utilizando Docker e Docker Compose, integrando Frontend, Backend, Base de Dados e um Proxy Reverso.

🚀 Arquitetura do Sistema

A solução é composta por 5 serviços principais:

Nginx (Porta 9000): Atua como Proxy Reverso, centralizando o acesso ao Frontend e à API.

Frontend (React/Vite): Interface do utilizador.

Backend (NestJS): API de serviços.

PostgreSQL: Base de dados relacional para persistência de dados.

pgAdmin: Interface gráfica para gestão da base de dados.

🛠️ Requisitos

Docker instalado

Docker Compose instalado

📦 Como Executar

Certifique-se de que o ficheiro .env está presente na raiz do projeto (baseado no .env.example).

No terminal, dentro da pasta raiz projeto-web, execute:

docker-compose up --build


Aguarde até que todos os containers estejam em estado de "running".

⚙️ Funcionalidades Implementadas

Orquestração Única: Todo o ambiente sobe com apenas um comando.

Hot-Reload: Graças ao mapeamento de volumes, qualquer alteração no código fonte do Frontend ou Backend é refletida instantaneamente sem necessidade de novo build.

Persistência de Dados: Utilização de volumes nomeados para garantir que os dados do PostgreSQL e as configurações do pgAdmin não sejam perdidos ao parar os containers.

Isolamento de Rede: Todos os serviços comunicam através de uma rede interna bridge personalizada.

Trabalho prático desenvolvido para a disciplina de Tecnologias de Software.
