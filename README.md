# 📱 Gerador de QR Code com Docker

Este projeto é um gerador de QR Code simples e funcional, desenvolvido como parte de um desafio da plataforma **DIO (Digital Innovation One)**. A aplicação utiliza HTML, CSS e JavaScript puro para interagir com uma API externa e gerar códigos em tempo real.

O diferencial deste repositório é a infraestrutura utilizando **Docker** com o servidor **Apache (httpd)**, facilitando o deploy e a padronização do ambiente de desenvolvimento.

## 🚀 Tecnologias Utilizadas

* **Frontend:** HTML5, CSS3 e JavaScript (ES6+).
* **Estilização:** Fontes integradas via Google Fonts (Roboto).
* **API:** [QR Server API](https://goqr.me/api/) para geração dinâmica das imagens.
* **Infraestrutura:** Docker e Docker Compose.
* **Servidor Web:** Apache HTTP Server (imagem oficial `httpd:latest`).

## 🛠️ Como Executar com Docker

Para rodar o projeto localmente sem precisar instalar um servidor manualmente, siga os passos abaixo:

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/tavssl/docker-projeto1-dio.git](https://github.com/tavssl/docker-projeto1-dio.git)
    cd docker-projeto1-dio
    ```

2.  **Suba o container:**
    Certifique-se de que você está na pasta onde reside o arquivo `docker-compose.yml` (geralmente na pasta `compose/`).
    ```bash
    docker-compose up -d
    ```

3.  **Acesse no navegador:**
    A aplicação estará disponível em: `http://localhost:80`

## 📂 Estrutura de Pastas

```plaintext
docker-projeto1-dio/
├── docker-compose.yml   # Configuração do serviço Apache
├── website/                 # Arquivos estáticos da aplicação
│   ├── index.html
│   ├── css/
│   │   └── styles.css
│   ├── js/
│   │   └── scripts.js
│   └── img/
└── README.md
