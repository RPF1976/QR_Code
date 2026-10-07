# QR Fácil — Gerador de QR Code

Site 100% gratuito e privado para gerar QR Codes que **qualquer celular lê apontando a câmera** — sem app extra.

Acesse em `http://localhost:3000` após:

```bash
python3 -m http.server 3000 --bind 0.0.0.0
```

## ✅ Novo: Salvar em JPG com 3 Tamanhos

Agora o usuário entra no site, gera o QR e clica em um dos 3 botões de download em **JPG**:

- **PQ • Pequeno — 400×400 px (~120 KB)** → ideal para WhatsApp, Stories, assinatura de e-mail
- **MD • Médio — 800×800 px (~350 KB)** → **recomendado** para cardápio, mesa, adesivo
- **GD • Grande — 1200×1200 px (~780 KB)** → para cartaz, banner, gráfica/outdoor

Todos em `.jpg` com qualidade alta (92%), fundo branco sólido (JPG não suporta transparência) e nome automático `qrcode-pq-400x400-...jpg`.

Ainda disponíveis: **PNG** (com transparência opcional) e **SVG** vetorial.

## Funcionalidades

- **6 modos**: Texto livre, Link/URL, WhatsApp (`wa.me`), Wi-Fi (conexão automática), PIX (BR Code Banco Central) e E-mail
- **Prévia ao vivo** — digita e já vê o QR
- **Personalização**: correção de erro (L/M/Q/H), cores, margem, tamanho da prévia (256–1024 px)
- **Ações**: Copiar imagem, Imprimir, Compartilhar (Web Share API)
- **Privacidade total**: geração 100% no navegador, nada vai para servidor

## Como usar

1. Escolha o tipo (Texto, Link...)
2. Digite o conteúdo
3. Veja a prévia ao lado
4. Clique em **PQ / MD / GD** em "Salvar em JPG" — o arquivo baixa na hora
5. Teste: abra a câmera do celular e aponte

## Tecnologias

- HTML / CSS / JS puro
- `qrcode` (soldair/node-qrcode) via CDN — `QRCode.toCanvas` + `canvas.toBlob('image/jpeg')`
- Sem build

## Licença

MIT
