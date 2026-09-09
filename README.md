# ☕ Livraria Café com Chá

Site institucional de uma livraria-cafeteria fictícia, desenvolvido como **trabalho da matéria de Desenvolvimento Front-end**.

O projeto é construído **apenas com HTML e CSS** — sem JavaScript, sem frameworks, sem bibliotecas externas e sem imagens externas (as capas dos livros são desenhadas com CSS puro).

---

## 🎯 Objetivo do trabalho

Aplicar na prática os conteúdos de HTML semântico e CSS:

- estrutura semântica (`header`, `nav`, `main`, `section`, `article`, `footer`);
- estilização com um único arquivo CSS externo, compartilhado por todas as páginas;
- variáveis CSS (`:root`), Flexbox, CSS Grid e pseudo-elementos;
- layout responsivo com *media queries*;
- acessibilidade básica (contraste, `alt`, foco visível, `lang="pt-BR"`).

---

## 📁 Estrutura de arquivos

```
Livraria-Cafe-com-Cha/
├── index.html              # Home  (responsável: colega de equipe)
├── best-sellers.html       # Mais vendidos
├── recomendacoes.html      # Recomendações da Casa
├── css/
│   └── estilo.css          # CSS único, compartilhado por todas as páginas
└── README.md
```

Todas as páginas usam **o mesmo arquivo CSS** (`css/estilo.css`), para que o
site fique visualmente igual do início ao fim. O arquivo é organizado em
seções numeradas (variáveis, cabeçalho, botões, cada página, responsivo) para
facilitar encontrar e editar uma parte sem mexer nas outras.

---

## 👥 Divisão das tarefas

| Página | Arquivo HTML | Responsável |
| --- | --- | --- |
| Home | `index.html` | Colega de equipe |
| Mais Vendidos | `best-sellers.html` | Eduardo Lopes |
| Recomendações da Casa | `recomendacoes.html` | Eduardo Lopes |

O CSS (`css/estilo.css`) é compartilhado — qualquer alteração nele afeta
todas as páginas ao mesmo tempo, então vale avisar no grupo antes de mexer
nas seções que não são só suas.

---

## 🎨 Identidade visual

Como o CSS é único, a paleta e a tipografia já são as mesmas em todas as
páginas automaticamente — não precisa copiar nada. As variáveis ficam no
topo de `css/estilo.css`, dentro do bloco `:root`:

```css
:root {
  --cafe-escuro:  #3b2417;  /* textos e rodapé          */
  --cafe-medio:   #6f4b32;  /* títulos secundários      */
  --creme:        #f7f1e7;  /* fundo das páginas        */
  --creme-claro:  #fffdf9;  /* fundo dos cards          */
  --dourado:      #c08a4a;  /* destaques e botões       */
  --verde-cha:    #6b7f5e;  /* detalhes / selos         */
  --borda:        #e3d5c2;
}
```

| Cor | Hex | Uso |
| --- | --- | --- |
| Café escuro | `#3b2417` | Texto principal, rodapé |
| Café médio | `#6f4b32` | Subtítulos, textos de apoio |
| Creme | `#f7f1e7` | Fundo geral |
| Dourado | `#c08a4a` | Botões, links de destaque, numeração |
| Verde chá | `#6b7f5e` | Selos e detalhes |

**Fontes:** `Georgia, 'Times New Roman', serif` para títulos e
`'Segoe UI', Tahoma, Verdana, sans-serif` para textos (fontes do sistema, sem
depender de internet).

**Menu de navegação (mesmo em todas as páginas):**

```html
<nav class="menu">
  <a href="index.html">Início</a>
  <a href="best-sellers.html">Mais Vendidos</a>
  <a href="recomendacoes.html">Recomendações da Casa</a>
</nav>
```

Na página em que o link estiver ativo, adicione `class="menu__ativo"` a ele
(ex.: `<a href="index.html" class="menu__ativo">Início</a>` na home).

> ⚠️ Para a home entrar no mesmo padrão, o `<head>` de `index.html` também
> precisa carregar o CSS único do projeto:
> `<link rel="stylesheet" href="css/estilo.css">`

---

## ▶️ Como visualizar

1. Clone ou baixe o repositório;
2. Abra qualquer arquivo `.html` diretamente no navegador (duplo clique);
3. Não é necessário servidor, instalação ou build.

---

## 📱 Responsividade

As páginas funcionam em telas de celular, tablet e desktop. Os *breakpoints*
usados são:

- até `640px` — layout em uma coluna (celular);
- de `641px` a `960px` — duas colunas (tablet);
- acima de `960px` — layout completo (desktop).

---

## 📌 Observações

- Projeto acadêmico e sem fins comerciais; livros, preços e depoimentos são fictícios.
- Nenhuma imagem externa é usada: as capas são feitas com `linear-gradient` e
  pseudo-elementos, para o site funcionar mesmo offline.

---

Trabalho da disciplina **Desenvolvimento Front-end**.
