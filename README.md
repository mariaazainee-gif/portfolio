# Portfólio — Maria Zaine

## Estrutura de pastas

```
portfolio/
├── index.html          → estrutura e conteúdo da página
├── css/
│   └── style.css       → todo o estilo visual (cores, fontes, espaçamentos)
├── assets/
│   ├── img/             → coloque aqui fotos e prints dos projetos
│   └── icons/           → coloque aqui ícones extras, se quiser usar
└── README.md            → este arquivo
```

## Como abrir e editar no VS Code

1. Abra a pasta `portfolio` inteira no VS Code (File → Open Folder).
2. Instale a extensão **Live Server** (procure por "Live Server" na aba de extensões).
3. Clique com o botão direito em `index.html` → **Open with Live Server**.
   O navegador abre a página e atualiza sozinha a cada vez que você salvar um arquivo.

## Como adicionar sua foto

1. Salve a imagem em `assets/img/` (ex: `assets/img/foto-perfil.jpg`).
2. Abra `index.html`, procure o comentário `<!-- Pra colocar sua foto -->` dentro do `<div class="avatar-wrap">`.
3. Siga as instruções do comentário: é só trocar o `<span>M</span>` por uma tag `<img>` apontando pro arquivo.

O mesmo vale para prints dos projetos: cada projeto na seção "Projetos" tem um comentário parecido mostrando onde encaixar a imagem.

## Como mudar as cores e o CSS

Tudo que é cor está centralizado no topo do arquivo `css/style.css`, dentro de `:root`:

```css
:root{
  --violet:#5B3A9E;
  --coral:#FF6B4A;
  --teal:#1FAE9A;
  ...
}
```

Mudando esses valores, a cor muda no site inteiro (botões, links, textos de destaque). Pra ajustar espaçamentos, fontes ou qualquer outro estilo, é só editar a regra correspondente mais abaixo no mesmo arquivo — cada seção do CSS está com um comentário indicando a que parte da página ela pertence.

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (ex: `portfolio` ou `meu-portfolio`).
2. Suba o conteúdo desta pasta pra ele (pelo VS Code, pelo terminal com `git`, ou arrastando os arquivos pela interface do GitHub).
3. No repositório, vá em **Settings → Pages**.
4. Em "Branch", selecione `main` (ou `master`) e a pasta `/ (root)`, depois salve.
5. Em alguns minutos o GitHub te dá um link tipo `https://seu-usuario.github.io/nome-do-repositorio/` com o site no ar.

## Pendências que você já sabe

- Trocar o e-mail placeholder (`seuemail@exemplo.com`) pelo seu e-mail real, no rodapé do `index.html`.
- Adicionar sua foto (veja acima).
- Adicionar prints dos projetos, se quiser.
