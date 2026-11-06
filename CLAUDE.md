# CLAUDE.md

Site GitHub Pages com páginas de suporte e políticas de privacidade das apps Android.

## Regra principal de manutenção
Sempre que alterares o site, mantém `README.md` (tabela de URLs, estrutura) e este `CLAUDE.md` atualizados.

## Regras
- HTML e CSS puros. Sem build, sem Jekyll, sem frameworks, sem JavaScript.
- **Sem recursos de terceiros** (fontes, CDNs, analytics, embeds): as políticas dizem que não há recolha de dados, e o site tem de ser coerente com isso.
- Todas as páginas em PT-PT, com secção inglesa no fim em `<section id="en" lang="en">`.
- Caminhos relativos entre páginas (`../assets/...`). Exceção: `404.html` usa caminhos absolutos a partir da raiz (`/assets/...`), porque é um site de utilizador.
- Os **URLs publicados nunca mudam** (estão registados na Play Console). Não renomear pastas nem ficheiros `privacy.html`.
- A política de privacidade de cada app tem de refletir o comportamento real da app. Se a app mudar (nova permissão, analytics, anúncios, contas, rede), atualizar a política **e a data "Última atualização"** em PT e EN.
- Apps com contas de utilizador precisam também de uma página de eliminação de conta (`<app>/delete-account.html`), exigida pela Google Play.

## Apps
| Slug | App | Notas para a política |
|---|---|---|
| `instant-barcode` | Instant Barcode | Sem dados recolhidos; leitura via Google Code Scanner (Play Services), sem permissão CAMERA; guardar na galeria (WRITE_EXTERNAL_STORAGE só API ≤ 28) e partilhar via folha do Android |

## Placeholders por preencher
`[NOME]` (nome de programador da Play Console) — substituir em todos os ficheiros antes de publicar.

## Conta
- GitHub: `milheirodev-creator`, repositório `milheirodev-creator.github.io` → https://milheirodev-creator.github.io/
- Contacto público: milheiro.dev@gmail.com
