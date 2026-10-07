# QR Fácil — Gerador de QR Code

Site 100% gratuito e privado para gerar QR Codes que **qualquer celular lê apontando a câmera** — sem app extra.

Acesse o site rodando localmente:

```bash
python3 -m http.server 3000 --bind 0.0.0.0
# abra http://localhost:3000
```

## Funcionalidades

- **6 modos**: Texto livre, Link/URL, WhatsApp (`wa.me`), Wi-Fi (conexão automática), PIX (BR Code padrão Banco Central) e E-mail
- **Prévia ao vivo** — digita e já vê o QR Code
- **Baixar em PNG (alta resolução até 1024px) e SVG vetorial**
- **Copiar imagem** e **Compartilhar** (Web Share API)
- **Personalização**: tamanho, nível de correção (L/M/Q/H), cores, fundo transparente e margem
- **Privacidade total**: tudo é gerado no seu navegador, nada vai para servidor
- **Impressão** otimizada

## Como usar

1. Escolha o tipo (Texto, Link, etc.)
2. Digite o conteúdo
3. Ajuste tamanho/cores se quiser
4. Clique em **Baixar PNG** ou **Copiar imagem** e cole onde quiser — cardápio, cartaz, mesa, embalagem

Dica: no iPhone e Android novos é só abrir a câmera e apontar.

## Tecnologias

- HTML / CSS / JS puro
- `qrcode` (https://github.com/soldair/node-qrcode) via CDN — geração em `canvas`
- Sem build, sem dependências

## Licença

MIT
