# Site do Kudondza Center

Página única, em HTML e CSS, sem compilação nem dependências. Foi feita primeiro para telemóvel e carrega bem com rede fraca: as imagens somam menos de 80 KB.

## Ver localmente

Abrir `index.html` no navegador. Também funciona sem Internet; nesse caso aparecem as letras do sistema em vez das do Google Fonts.

## Publicação (GitHub Pages)

Endereço: **<https://duarte-mondlane.github.io/kudondza/>**

O site é publicado pelo fluxo [`.github/workflows/pages.yml`](../.github/workflows/pages.yml). Corre sozinho sempre que entra no `main` uma alteração à pasta `site/`. Também se pode correr à mão em **Actions → Publicar site → Run workflow**.

### Configuração inicial (uma só vez)

Em **Settings → Pages → Build and deployment → Source**, escolher **GitHub Actions** (não **Deploy from a branch**).

Se ficar em **Deploy from a branch**, o GitHub faz uma segunda publicação a cada alteração no `main`, a partir da raiz do repositório. Essa publicação termina depois da do fluxo, e o site fica a mostrar o `README.md` em vez da página.

### Domínio próprio (opcional)

Para usar um domínio como `kudondza.co.mz`: registá-lo, indicá-lo em **Settings → Pages → Custom domain** e configurar o DNS como o GitHub explicar nessa página. Depois, atualizar `canonical`, `og:url` e `og:image` no `index.html` com o novo endereço.

## Onde mudar o quê

| Para mudar | Onde |
|---|---|
| Datas, horários, local, preço | `index.html`, secção `como-funciona` e destaque inicial |
| Número de telefone ou WhatsApp | `index.html`: procurar `258879994892` (aparece em todos os botões) |
| Mensagem que chega pelo WhatsApp | `index.html`: o texto depois de `?text=` nos links `wa.me` |
| Cores e letras | `styles.css`, bloco `:root` no início do ficheiro |
| Fotografia e logótipo | `img/`; foram recortados do flyer e podem ser trocados por fotografias reais |
