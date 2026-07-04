# 💇‍♀️ Franja Torta Studio

Site oficial do **Franja Torta Studio** — um estúdio de cabelo alternativo, com identidade visual inspirada em colagem, zine e adesivos rasgados.

🔗 **Site no ar:** https://franjatorta.github.io/studio.franjatorta/
📷 **Instagram:** [@franjatorta.studio](https://www.instagram.com/franjatorta.studio/)

---

## ✂️ Sobre o projeto

Este repositório contém o site institucional do Franja Torta Studio: uma página única (single-page) com identidade visual autoral, apresentando o estúdio, os serviços, a galeria de trabalhos, depoimentos e os canais de agendamento.

O site é **estático** (HTML, CSS e JavaScript puro, sem frameworks) e publicado gratuitamente via **GitHub Pages**. A galeria de fotos é editável através de um painel de administração simples, sem precisar mexer em código.

## 🗂️ Estrutura de arquivos
├── index.html              # página principal do site
├── logo.png                # logo do estúdio
├── admin/
│   ├── index.html          # carrega o painel de administração (Decap CMS)
│   └── config.yml          # configuração do painel (conexão com o GitHub)
├── content/
│   └── galeria.json        # dados das fotos da galeria (editado pelo painel)
└── images/
    └── galeria/            # fotos enviadas pelo painel ficam salvas aqui

- O site é 100% estático e hospedado no **GitHub Pages**, direto a partir da branch `main`.
- A seção **Galeria** carrega as fotos dinamicamente a partir do arquivo `content/galeria.json` via JavaScript.
- Para editar as fotos sem mexer em código, existe um painel de administração feito com **[Decap CMS](https://decapcms.org/)**, acessível em:
  👉 `https://zippy-lamington-c1a549.netlify.app/admin/`
- O login do painel usa sua conta do **GitHub** como autenticação (via um app OAuth conectado a um projeto na Netlify, que serve apenas como intermediário de login — o site continua hospedado só no GitHub Pages).
- Toda alteração feita no painel gera automaticamente um commit neste repositório, e o site atualiza sozinho em poucos minutos.
