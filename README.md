# Documentação da Nikkita

Site de documentação da Nikkita, publicado em [docs.nikkita.com.br](https://docs.nikkita.com.br) e construído com [Mintlify](https://mintlify.com).

## Estrutura

- `docs.json` — configuração do site: navegação, tema, logo e links
- `index.mdx` — página de boas-vindas (tab **Comece aqui**)
- `introducao.mdx`, `como-funciona.mdx`, `primeiros-passos.mdx` — tab **Documentação**
- `images/` — logo e favicon
- `AGENTS.md` — instruções de estilo e contexto para ferramentas de IA

## Rodar localmente

Instale a CLI do Mintlify:

```
npm i -g mint
```

Na raiz do repositório, onde fica o `docs.json`:

```
mint dev
```

O preview roda em `http://localhost:3000`.

## Publicar

O app do GitHub do Mintlify propaga o repositório para o deploy. Alterações no branch `main` vão para produção automaticamente.

## Problemas comuns

- Ambiente de dev não sobe: rode `mint update` para atualizar a CLI.
- Página carrega como 404: confirme que você está na pasta com um `docs.json` válido e que o slug está listado em `navigation`.
