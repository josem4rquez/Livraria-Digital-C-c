# ☕ Livraria Café com Chá

Site institucional de uma livraria-cafeteria fictícia, desenvolvido como **trabalho da matéria de Desenvolvimento Front-end**.

O projeto é construído **apenas com HTML e CSS** — sem JavaScript, sem frameworks, sem bibliotecas externas e sem imagens externas (as capas dos livros são desenhadas com CSS puro).

---

## 🎯 Objetivo do trabalho

Aplicar na prática os conteúdos de HTML semântico e CSS:

- estrutura semântica (`header`, `nav`, `main`, `section`, `article`, `footer`);
- estilização com CSS externo (um arquivo `.css` por página);
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
│   ├── index.css           # Estilo da Home
│   ├── best-sellers.css    # Estilo da página de Mais Vendidos
│   └── recomendacoes.css   # Estilo da página de Recomendações
└── README.md
```

Cada página tem **seu próprio arquivo HTML e seu próprio arquivo CSS**, para que as
partes possam ser desenvolvidas separadamente e unidas no final sem conflitos.

---

## 👥 Divisão das tarefas

| Página | Arquivos | Responsável |
| --- | --- | --- |
| Home | `index.html` + `css/index.css` | Colega de equipe |
| Mais Vendidos | `best-sellers.html` + `css/best-sellers.css` | Eduardo Lopes |
| Recomendações da Casa | `recomendacoes.html` + `css/recomendacoes.css` | Eduardo Lopes |

---

## 🎨 Identidade visual (padrão para todas as páginas)

Para que as páginas fiquem consistentes depois de unidas, todas usam a mesma
paleta e a mesma tipografia. Basta copiar o bloco `:root` abaixo no início do CSS
de cada página.

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
