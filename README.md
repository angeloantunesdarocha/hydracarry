<div align="center">

# 🚰 HydraCarry

**Carregue sua garrafa sem usar as mãos.**

Uma landing page moderna e responsiva para o **HydraCarry** — uma bolsa transversal desenvolvida para acompanhar seu copo tumbler (Stanley, Owala, HydroJug e similares), mantendo também seu celular, chaves e cartões sempre à mão.

🔗 **[hydracarry.vercel.app](https://hydracarry.vercel.app)**

</div>

---

## ✨ Visão Geral

HydraCarry é uma bolsa transversal (*crossbody bag*) focada em praticidade e estilo. O site foi construído para apresentar o produto, reunir interessados em acesso antecipado e gerar uma lista de espera antes do lançamento oficial.

O projeto demonstra um fluxo completo de desenvolvimento web: do design até o deploy em produção.

---

## 🎯 Funcionalidades

- 🎨 **Design responsivo** — adaptável de mobile a desktop
- 🖼️ **Galeria interativa** com 6 fotos do produto e visualizador em tela cheia (*lightbox*)
- ⚡ **Carregamento otimizado** com *lazy loading* e animação de entrada via `IntersectionObserver`
- ⌨️ **Acessibilidade** — navegação por teclado (setas, *Esc*), `aria-labels` e contraste adequado
- 📧 **CTA de contato** integrado via `mailto` para captura de leads
- 🌐 **Zero dependências externas** — HTML, CSS e JavaScript puro, sem frameworks

---

## 🛠️ Tecnologias

| Camada       | Tecnologia                |
| ------------ | ------------------------- |
| Marcação     | HTML5                     |
| Estilização  | CSS3 (variáveis, grid, animação) |
| Interação    | JavaScript (vanilla)      |
| Hospedagem   | [Vercel](https://vercel.com)               |
| Versionamento| Git + GitHub              |

---

## 📁 Estrutura do Projeto

```
hydracarry/
├── index.html              # Página principal
├── assets/
│   └── images/             # Galeria de imagens do produto
│       ├── hydracarry-01.png
│       ├── hydracarry-02.png
│       ├── hydracarry-03.png
│       ├── hydracarry-04.png
│       ├── hydracarry-05.png
│       └── hydracarry-06.png
└── README.md
```

---

## 🚀 Como Executar Localmente

Não há build, instalação de dependências ou etapa de compilação. Basta abrir o `index.html` no navegador:

```bash
# Opção 1 — abrir direto
start index.html         # Windows
open index.html          # macOS

# Opção 2 — servidor local (recomendado para inspecionar a galeria)
python -m http.server 8000
# Acesse http://localhost:8000
```

---

## 📷 Galeria

A galeria foi construída com **CSS Grid responsivo** e JavaScript vanilla:

- Grid que se adapta automaticamente ao tamanho da tela
- Efeito *hover* com zoom sutil e sombra expandida
- *Lightbox* modal com setas, *Esc* para fechar, e clique fora
- *Lazy loading* nativo (`loading="lazy"`)
- *Alt text* descritivo em todas as imagens para SEO

Para adicionar uma nova imagem, coloque o arquivo em `assets/images/` e adicione um bloco:

```html
<div class="gallery-item" data-index="6">
    <img src="assets/images/hydracarry-07.png" alt="Descrição" loading="lazy">
</div>
```

---

## 🎨 Paleta de Cores

| Uso                | Cor       |
| ------------------ | --------- |
| Primária           | `#0A4F60` |
| Primária (hover)   | `#0C6478` |
| Fundo de seções    | `#f5f5f5` |
| Fundo de cards     | `#f0f8fa` |
| Texto principal    | `#333333` |

---

## 👤 Autor

Desenvolvido por **[Ângelo Antunes](https://github.com/angeloantunesdarocha)**

Contato para o projeto: **angeloantunesdarocha@gmail.com**

---

## 📄 Licença

© 2026 HydraCarry. Todos os direitos reservados.
