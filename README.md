# Portfólio | Felipe

Projeto desenvolvido para mostrar trabalhos, meios de contato e projetos do GitHub.
**Node.js (Express)** servindo a pasta estática `public/`.

## Estrutura

- **`public/`** – HTML, CSS, imagens e assets do portfólio
- **`server.js`** – Servidor Express (Node.js) para desenvolvimento local
- **`package.json`** – Dependências (express)

## Rodar localmente (Node.js)

```bash
npm install
npm start
```

Acesse **http://localhost:3000**

## Deploy no Vercel

Consulte **[DEPLOY.md](DEPLOY.md)** para instruções completas.

1. Envie o repositório para o GitHub
2. Conecte ao [Vercel](https://vercel.com/new)
3. O `vercel.json` já está configurado (output: `public`)

## Adicionar Projetos

Edite `public/index.html` e duplique um bloco `<div class="project-card">`. Atualize:
- **Imagem**: coloque o print em `public/images/` e altere o `src`
- **Título, descrição, tags** e **link do GitHub**
