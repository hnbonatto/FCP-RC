# F*CK PACE Running Club — Landing (Drop 2)

Landing de pré-venda. HTML/CSS/JS estático, sem build — pronto pra GitHub Pages.

## IMPORTANTE — estrutura plana (tudo na raiz)
Todos os arquivos ficam na **raiz** do repositório, no mesmo nível (sem subpastas).
Os caminhos das imagens são relativos à raiz (ex.: `mc-branca-full-cut.png`), então
basta subir todos os arquivos juntos.

## Deploy (GitHub Pages)
1. Suba TODOS os arquivos desta pasta para a **raiz** do repositório (sem criar subpastas).
2. Settings → Pages → Source: **Deploy from a branch** → branch `main`, pasta `/ (root)`.
3. Aguarde ~1 min o build e acesse `https://<usuario>.github.io/<repo>/`.
   (Se aparecer 404 logo após configurar, espere o build terminar e dê um hard-refresh: Ctrl+Shift+R.)

`index.html` é o ponto de entrada.

## Arquivos
```
index.html                  → página principal (banner + formulário de pedidos)
banner.html                 → hero (iframe ?embed=1)
globe.html                  → globo wireframe 3D (iframe ?bare=1, dentro do banner)
product-loop.html           → preview animado das camisetas (?product=<cor>&mini=1)
orders.css                  → estilos do formulário
*-full-cut.png              → arte das costas (mc/ml × preta/branca)
*-nowordmark-cut.png        → frame do glitch (sem o wordmark)
*-alt-cut.png               → frente com logo pequeno
.nojekyll                   → desativa o Jekyll do GitHub Pages
```

## Dependências externas (precisam de internet)
- **xlsx** (exportação Excel do pedido) — CDN cdnjs.
- **Imagens dos bonés** — CDN do Google Forms.
- **Google Fonts** (Archivo Black, Space Grotesk, Space Mono).

## Observações
- Os pedidos são salvos no `localStorage` do navegador e um `.xlsx` é baixado ao confirmar
  (não há backend). Para receber pedidos de verdade, conecte um backend ou serviço de formulário.
