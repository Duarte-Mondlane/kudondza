# Site do Kudondza Center

Página única, em HTML e CSS, sem compilação nem dependências. Foi feita primeiro para telemóvel e carrega bem com rede fraca: as imagens somam menos de 80 KB.

## Ver localmente

Abrir `index.html` no navegador. Também funciona sem Internet; nesse caso aparecem as letras do sistema em vez das do Google Fonts.

## Publicar (Cloudflare Pages, gratuito)

O repositório é privado, e o GitHub Pages só publica repositórios privados em planos pagos. O Cloudflare Pages publica de graça a partir de um repositório privado.

1. Criar uma conta em <https://dash.cloudflare.com/sign-up>.
2. Em **Workers & Pages**, criar um projeto **Pages** ligado ao Git (*Connect to Git*) e autorizar o acesso ao repositório `Duarte-Mondlane/kudondza`.
3. Configurar:
   - **Production branch:** `main`
   - **Framework preset:** None
   - **Build command:** deixar vazio
   - **Build output directory:** `site`
4. Guardar. O site fica disponível num endereço do tipo `https://kudondza.pages.dev`.

A partir daí, cada alteração enviada para o `main` atualiza o site automaticamente. Alterações noutros ramos geram um endereço de pré-visualização à parte.

### Depois de publicar

Na linha `og:image` do `index.html`, trocar `img/pratica.jpg` pelo endereço completo, por exemplo `https://kudondza.pages.dev/img/pratica.jpg`. Sem isso, o WhatsApp e o Facebook não mostram a imagem quando o link é partilhado.

## Onde mudar o quê

| Para mudar | Onde |
|---|---|
| Datas, horários, local, preço | `index.html`, secção `como-funciona` e destaque inicial |
| Número de telefone ou WhatsApp | `index.html`: procurar `258879994892` (aparece em todos os botões) |
| Mensagem que chega pelo WhatsApp | `index.html`: o texto depois de `?text=` nos links `wa.me` |
| Cores e letras | `styles.css`, bloco `:root` no início do ficheiro |
| Fotografia e logótipo | `img/`; foram recortados do flyer e podem ser trocados por fotografias reais |
