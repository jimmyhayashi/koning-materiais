# Koning Materiais de Construção — Site

Site institucional estático (HTML, CSS e JavaScript puro — sem dependências).
Em português do Brasil. Pronto para publicar em qualquer hospedagem estática.

## Estrutura

```
index.html        → página única com todas as seções
styles.css        → identidade visual (azul-marinho + ciano, do logo) e responsividade
script.js         → menu mobile e ano do rodapé
assets/img/       → logo, foto do hero e favicon
```

## Seções
- **Topo / Hero** — nome da loja, slogan e botões de WhatsApp/produtos
- **Diferenciais** — loja ampla, atendimento, preço justo
- **A Loja (Sobre)** — história desde 2008 e reinauguração em 2024
- **Produtos** — categorias (construção, ferragens, ferramentas, elétrica, hidráulica, tintas)
- **Horários** — funcionamento
- **Contato** — WhatsApp, telefone fixo, Instagram, endereço e mapa do Google
- **Botão flutuante** de WhatsApp em todas as telas

## Como personalizar

### 1. Logo real
Coloque o arquivo em `assets/img/logo.png` e, no `index.html`, troque o bloco do
logo (a “coroa”) descomentando a linha:

```html
<img src="assets/img/logo.png" alt="Koning Materiais de Construção" class="brand__img">
```

...e removendo o `<span class="brand__mark">...</span>` e o `<span class="brand__text">...</span>`.

### 2. Foto do hero (fundo do topo)
Salve uma foto boa da loja/fachada como `assets/img/hero.jpg`.
O CSS já aponta para ela automaticamente (em `.hero`). Enquanto não houver foto,
o fundo usa um gradiente azul com textura — já fica apresentável.

### 3. Dados que podem mudar
Telefones, WhatsApp, horários e endereço estão no `index.html`. Links do WhatsApp
usam o formato `https://wa.me/5547997201961`.

## Publicar (grátis)
Qualquer uma destas opções funciona por ser um site estático:
- **Netlify** / **Vercel** / **Cloudflare Pages** — arraste a pasta ou conecte o Git
- **GitHub Pages** — ative nas configurações do repositório
- Hospedagem tradicional — envie os arquivos por FTP

## Visualizar localmente
Basta abrir o `index.html` no navegador, ou rodar um servidor simples:

```bash
python3 -m http.server 8000
# abra http://localhost:8000
```
