# Deploy no Vercel

## Pré-requisitos

1. **Imagens**: Copie as imagens do projeto ASP.NET para a pasta estática:
   ```
   Portifolio\wwwroot\images\  →  public\images\
   ```
   (Arquivos: 6.png, 7.png, 8.png)

2. **Conta no Vercel**: [vercel.com](https://vercel.com)

## Deploy

### Opção 1: Via GitHub (recomendado)

1. Envie o projeto para um repositório no GitHub
2. Acesse [vercel.com/new](https://vercel.com/new)
3. Importe o repositório
4. O Vercel detectará automaticamente o `vercel.json`
5. **Root Directory**: deixe como está (ou defina como raiz do projeto)
6. **Output Directory**: `public` (já configurado no vercel.json)
7. Clique em Deploy

### Opção 2: Via Vercel CLI

```bash
npm i -g vercel
vercel
```

Siga as instruções. O site estático será servido da pasta `public/`.

## Estrutura para adicionar projetos

Para adicionar um novo projeto, duplique um bloco `<article class="project-card">` em `public/index.html` e edite:

| Campo | Onde editar |
|-------|-------------|
| **Screenshot** | `src="images/SEU_PRINT.png"` - coloque o print na pasta `public/images/` |
| **Título** | `<h3 class="project-card-title">Nome do Projeto</h3>` |
| **Descrição** | `<p class="project-card-desc">...</p>` |
| **Link GitHub** | `href="https://github.com/USUARIO/REPO"` no `.project-link` |
| **Tags** | `<span class="project-tag">C#</span>` - adicione/remova conforme as tecnologias |

## Nota sobre ASP.NET

O Vercel não suporta aplicações ASP.NET Core nativamente. Esta pasta `public/` contém uma versão **estática** (HTML/CSS/JS) do portfólio, otimizada para o Vercel. O projeto em `Portifolio/` continua disponível para desenvolvimento local com `dotnet run`.
