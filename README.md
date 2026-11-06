# Páginas das apps (GitHub Pages)

Site estático com as páginas que a Google Play exige para cada app: **política de privacidade** e **página de suporte**.
HTML + CSS simples, sem build, sem Jekyll (`.nojekyll`), sem fontes nem scripts de terceiros.

## URLs

Repositório `milheirodev-creator.github.io` na conta `milheirodev-creator` (site de utilizador, servido na raiz):

| App | Suporte | Privacidade (usar na Play Console) |
|---|---|---|
| Instant Barcode | `https://milheirodev-creator.github.io/instant-barcode/` | `https://milheirodev-creator.github.io/instant-barcode/privacy.html` |

## Publicar

1. Criar o repositório **público** `milheirodev-creator.github.io` e fazer push deste conteúdo para `main`.
2. **Settings → Pages → Build and deployment → Source: Deploy from a branch → `main` / `(root)`**.
3. Esperar 1–2 minutos e abrir os URLs acima (sem sessão iniciada, para confirmar que são públicos).

## Estrutura

```
index.html                 # lista de apps
404.html
assets/style.css           # estilo comum (cor da app via --app)
assets/<app>.png           # ícone de cada app
<app>/index.html           # suporte: descrição, FAQ, contacto (PT + EN)
<app>/privacy.html         # política de privacidade (PT + EN)
```

## Adicionar uma app

1. Copiar a pasta `instant-barcode/` para `<nova-app>/` (slug curto, minúsculas, com hífens).
2. Pôr o ícone 512×512 em `assets/<nova-app>.png`.
3. Rever o texto de `privacy.html` para refletir **exatamente** o que a nova app faz com dados.
4. Se a app tiver outra cor, adicionar `style="--app:#XXXXXX"` ao `<header class="band">`.
5. Acrescentar a app em `index.html` e na tabela de URLs deste README.
