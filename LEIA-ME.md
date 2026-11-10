# Portfólio Daniel Cabral — deploy no Netlify

## O que trocar antes de publicar
1. **Vídeos**: nos `<iframe>`, troque `COLE_ID_...` pela URL de embed de cada vídeo.
   - YouTube: `https://www.youtube.com/embed/ID`
   - Vimeo: `https://player.vimeo.com/video/ID`
   - Verticais: suba como YouTube Shorts ou Vimeo (não listado). Evite Google Drive.
2. **Foto**: o código já aponta para `foto.jpg`. Salve a foto do Daniel com esse nome e coloque na pasta.
   (O vídeo LOTR 3 já está com o embed real do Vimeo preenchido.)
3. **Contatos**: troque `55DDDNUMERO` (WhatsApp) e `daniel@exemplo.com` (e-mail).
4. **Capa de compartilhamento**: crie `og-cover.jpg` (1200x630) e coloque na pasta.
5. **Domínio**: nas meta tags `og:url` e `og:image`, troque `SEU-DOMINIO.netlify.app`.

## Publicar
### Opção A — arrastar e soltar (mais rápido)
1. Entre em app.netlify.com → "Add new site" → "Deploy manually".
2. Arraste esta pasta. Pronto.

### Opção B — Git (deploy automático a cada push)
1. Suba a pasta num repositório GitHub.
2. No Netlify: "Add new site" → "Import from Git" → escolha o repo.
3. Build command: (vazio). Publish directory: `/` (ou a raiz).

### Opção C — CLI
```
npm i -g netlify-cli
netlify deploy --prod
```

## Formulário
O formulário de contato usa Netlify Forms (já configurado com `data-netlify="true"`).
Os envios aparecem no painel do Netlify em **Forms**. Grátis até 100 envios/mês.
