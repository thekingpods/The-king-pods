# The King Pods

Loja online em uma única página (`index.html`), sem build e sem dependências para instalar.

## Como usar
1. Envie esta pasta para um repositório no GitHub (`index.html` na raiz).
2. Publique o repositório em um serviço de hospedagem que permita lojas, por exemplo **Netlify**, **Cloudflare Pages** ou **Vercel** (conecte o repositório e publique a raiz, sem comando de build).
3. Use um domínio próprio com HTTPS.

> **Atenção:** o GitHub Pages não permite hospedar lojas online / e-commerce (regra do próprio GitHub).
> Use o GitHub só para guardar o código e publique em outro serviço.

## O que já vem configurado
- Pix com a chave, nome e cidade definidos no começo do script (`const PIX=...`).
- Frete: Loggi, Jadlog e Sedex, com preços e prazos em `const SHIP=...`.
- Produtos, preços e sabores em `const P=...` e `const FL=...`.
- Instagram da loja no rodapé, Termos de Uso e Política de Privacidade.

## Limites desta versão
- Contas, carrinho e pedidos ficam salvos **só no navegador de cada cliente** (não existe servidor).
- O dono da loja não vê a lista de clientes nem de pedidos, e o rastreio não muda de status sozinho.
- Para contas em qualquer aparelho, painel de pedidos e proteção de dados de verdade, é preciso ligar um banco de dados (ex.: Firebase ou Supabase) com regras de acesso.
- O QR code do Pix usa a biblioteca `qrcodejs` carregada do cdnjs (precisa de internet).
