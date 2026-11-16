# Portfólio · Letícia Beatriz

Site pessoal e vitrine do meu trabalho: sites, cardápios com pedido pelo WhatsApp, materiais e planilhas **simples e acessíveis** para pequenos negócios de todo o Brasil.

🔗 **No ar (endereço provisório):** https://portfolio-85x.pages.dev/

---

## Como o site é feito

- **HTML, CSS e um pouco de JavaScript**, tudo escrito à mão.
- **Sem dependências e sem etapa de build**: o que está no repositório é exatamente o que vai para o ar.
- **Uma página só (`index.html`)**. As páginas de cada serviço ficam dentro dela e abrem por endereço com âncora (`#servico-...`). Isso funciona bem no celular e no botão "voltar".
- **Fontes:** Fraunces (títulos), Atkinson Hyperlegible Next (texto, feita para ser fácil de ler) e Caveat (anotações à mão), todas do Google Fonts.
- **Desenhos:** feitos à mão por mim e vetorizados em `img/rabiscos.svg`.
- **Fotos:** recortes das minhas fotos e dos meus cachorros, em `.webp` para carregar rápido.

### O que tem na página

| Parte | O que faz |
|---|---|
| Topo | Apresentação com colagem de fotos. A Liza encolhe com a rolagem e vira a Liza que passeia pela página (só em telas grandes). |
| Serviços | Carrossel com os 6 serviços. Cada um tem uma página com o que inclui, o preço, o que o cliente envia e como funciona. |
| Calculadora | Mostra em quantos clientes o serviço se paga. |
| Pedido fora da lista | Monta uma mensagem pronta para WhatsApp ou e-mail. Nada fica salvo. |
| Perguntas frequentes | Chat com a Liza com respostas prontas sobre cerca de 50 assuntos (sem inteligência artificial e sem coletar dados). |
| Menu de acessibilidade | Aumenta a letra, aumenta o contraste, troca a fonte, para as animações e esconde os enfeites. As escolhas ficam salvas no navegador. |

---

## Acessibilidade

O site segue a **WCAG 2.2, nível AA**:

- contraste adequado em todas as cores;
- navegação completa pelo teclado, com foco visível;
- textos alternativos nas imagens (enfeites são ignorados pelo leitor de tela);
- títulos em ordem e regiões marcadas (cabeçalho, conteúdo, rodapé);
- respeita quem pede menos movimento no sistema (`prefers-reduced-motion`);
- funciona de 320 px de largura até telas grandes.

---

## Checklist antes de publicar uma mudança

1. **Validador W3C**: https://validator.w3.org/ (0 erros)
2. **WAVE**: https://wave.webaim.org/ (0 erros de acessibilidade)
3. **PageSpeed Insights**: https://pagespeed.web.dev/ (celular e computador)
4. **Teste em 2 celulares** de verdade: menu, carrossel, calculadora, perguntas e botões de WhatsApp.

---

## Estrutura dos arquivos

```
index.html     a página inteira (HTML, CSS e JavaScript)
404.html       página de "não encontrado"
img/           fotos, recortes, desenhos (rabiscos.svg) e imagem de compartilhamento
favicon.svg    ícone da aba
_headers       cache das imagens na Cloudflare
robots.txt     regras para buscadores
sitemap.xml    lista de páginas para o Google
```

---

## Publicação (Cloudflare Pages)

O site publica sozinho: **toda alteração enviada para a branch `main` vai para o ar em cerca de 1 minuto.**

Configuração do projeto na Cloudflare, para refazer se precisar:

1. Cloudflare → **Workers & Pages** → Create → Pages → **Connect to Git**.
2. Escolha o repositório `portfolio`.
3. Framework preset: **None**. Build command: deixe vazio. Output directory: `/`.
4. **Save and Deploy**.

Para contar visitas sem cookies: no projeto, vá em **Metrics** e clique em **Enable** em Web Analytics.

### Ao trocar o endereço do site

Atualize o endereço novo nestes lugares:
- `index.html`: `<link rel="canonical">`, as tags `og:url` e `og:image` e a ficha do Google (`application/ld+json`);
- `sitemap.xml` e `robots.txt`.

---

## Direitos

O código pode servir de inspiração. **As fotos, os desenhos e os textos são meus** e não podem ser reutilizados sem autorização.

Feito à mão por Letícia Beatriz, com supervisão da Liza. 🐾
