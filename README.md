# Portfólio | Felipe

Projeto desenvolvido para mostrar trabalhos, meios de contato e projetos do GitHub.
Desenvolvido em C# com .NET (versão local) e versão estática para deploy no Vercel.

## Estrutura

- **`Portifolio/`** – Projeto ASP.NET Core (desenvolvimento local: `dotnet run`)
- **`public/`** – Site estático para deploy no **Vercel**

## Deploy no Vercel

Consulte **[DEPLOY.md](DEPLOY.md)** para instruções completas.

1. Envie o repositório para o GitHub
2. Conecte ao [Vercel](https://vercel.com/new)
3. O `vercel.json` já está configurado (output: `public`)

## Adicionar Projetos

Edite `public/index.html` e duplique um bloco `<article class="project-card">`. Atualize:
- **Imagem**: coloque o print em `public/images/` e altere o `src`
- **Título, descrição, tags** e **link do GitHub**
