# Suporte Smart Sorocaba

Site de vendas da loja Suporte Smart Sorocaba — celular no boleto, mostruário de celulares, fones, smartwatches e caixas de som.

Página estática única: [`site/index.html`](site/index.html). Sem build, sem dependências.

## Rodar local

```bash
python -m http.server 5173 -d site
```

Abrir http://localhost:5173.

## Publicar

Netlify, via GitHub Actions ([`.github/workflows/deploy-netlify.yml`](.github/workflows/deploy-netlify.yml)): cada push na `main` publica a pasta `site/`. Também dá para rodar na mão em Actions → Deploy no Netlify → Run workflow.

O site pode estar em qualquer conta Netlify. Configure em Settings → Secrets and variables → Actions:

- `NETLIFY_AUTH_TOKEN`: token pessoal da conta Netlify dona do site (User settings → Applications → Personal access tokens).
- `NETLIFY_SITE_ID`: ID do site (Site configuration → Site details → Project ID).

## Produtos

A lista do mostruário fica no objeto `P` no fim de `site/index.html`. Para adicionar um item, coloque a foto em `site/assets/img/<categoria>/` (`.webp`, ~720px de largura) e adicione `["Nome", "arquivo-sem-extensao"]` na categoria.

Contato da loja: (15) 99180-4185 — Rua da Penha, 857, Loja 03, Centro, Sorocaba.
