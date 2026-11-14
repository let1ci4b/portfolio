# Portfólio — Letícia Beatriz

Site estático (HTML + CSS + um pouco de JavaScript), sem dependências e sem build.

- `index.html` — a página inteira
- `img/` — fotos e recortes

## Publicar na Cloudflare Pages
1. Cloudflare → Workers & Pages → Create → Pages → Connect to Git.
2. Escolha o repositório `portfolio`.
3. Framework preset: **None**. Build command: deixe vazio. Output directory: `/`.
4. Save and Deploy. Toda alteração enviada para a branch `main` atualiza o site sozinha.
