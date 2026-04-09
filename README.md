# José Araujo — Portfolio Site
## Guia completo de montagem e deploy (do zero, grátis)

---

## 📁 Estrutura de arquivos

```
portfolio/
├── index.html          ← o site completo (este arquivo)
├── README.md           ← este guia
└── assets/             ← suas imagens (crie esta pasta!)
    ├── cover.png
    ├── web_screens.png
    ├── mobile_screens.png
    ├── 01_Section.png
    ├── 02_Section.png
    ├── 03_Section.png
    ├── 04_Section.png
    ├── 05_Section.png
    ├── 06_Section.png
    ├── 07_Section.png
    ├── 08_Section.png
    ├── 09_Section.png
    ├── 10_Section.png
    ├── 11_Section.png
    ├── 12_Section.png
    ├── 13_Section.png
    └── 14_Section.png
```

---

## 🖼️ PASSO 1 — Organizar as imagens

1. Na mesma pasta do `index.html`, crie uma pasta chamada exatamente `assets`
2. Coloque TODAS as imagens do case VOLL dentro da pasta `assets/`:
   - Os arquivos que você tem: `cover.png`, `web_screens.png`, `mobile_screens.png`, e os `01_Section.png` até `14_Section.png`
   - Os nomes devem ser **exatamente iguais** aos listados acima (case sensitive)

---

## 🐙 PASSO 2 — Criar conta no GitHub (gratuito)

1. Acesse **github.com** e clique em "Sign up"
2. Escolha um username (ex: `josearaujo-design` — este aparecerá na URL)
3. Confirme o e-mail
4. Escolha o plano **Free**

---

## 📦 PASSO 3 — Criar o repositório

1. No GitHub, clique no **"+"** no canto superior direito → **"New repository"**
2. Nome do repositório: `portfolio` (ou seu-nome.github.io para URL customizada)
3. Marque **"Public"** (obrigatório para hospedagem grátis)
4. Clique em **"Create repository"**

---

## ⬆️ PASSO 4 — Fazer upload dos arquivos

**Opção A (mais fácil — sem instalar nada):**
1. Na página do repositório criado, clique em **"uploading an existing file"**
2. Arraste **toda a pasta** (index.html + pasta assets com as imagens)
3. Escreva uma mensagem de commit: "Initial portfolio upload"
4. Clique em **"Commit changes"**

**Opção B (mais profissional — Git):**
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/SEU-USERNAME/portfolio.git
git push -u origin main
```

---

## 🌍 PASSO 5 — Ativar o GitHub Pages (hospedagem gratuita)

1. No repositório, clique em **"Settings"** (engrenagem no menu superior)
2. No menu lateral esquerdo, clique em **"Pages"**
3. Em "Source", selecione **"Deploy from a branch"**
4. Em "Branch", selecione **"main"** e pasta **"/ (root)"**
5. Clique em **"Save"**
6. Aguarde ~2 minutos
7. Seu site estará em: **`https://SEU-USERNAME.github.io/portfolio`**

---

## 🔗 PASSO 6 (opcional) — Domínio customizado gratuito

Para ter uma URL como `josearaujo.design`:

**Opção grátis com Freenom** (domínios .tk, .ml):
- freenom.com → registrar domínio → apontar para GitHub Pages

**Opção paga mas barata** (~R$60/ano):
- Registro.br (domínio .com.br) ou Namecheap (domínio .com)
- No GitHub Settings > Pages > Custom domain: coloque seu domínio
- Na sua DNS, adicione: CNAME `www` → `SEU-USERNAME.github.io`

---

## 🚀 Alternativa: Deploy na Vercel (ainda mais fácil)

1. Acesse **vercel.com** → "Sign up with GitHub"
2. Clique em **"New Project"** → importe seu repositório
3. Clique em **"Deploy"**
4. Pronto! URL automática: `portfolio-seu-nome.vercel.app`
5. Atualizações automáticas: qualquer push no GitHub atualiza o site

---

## ✏️ Como editar o site

Tudo está em **um único arquivo** `index.html`. Para editar:

| O que mudar | Onde encontrar no HTML |
|---|---|
| Seu nome | `<h1 class="home-title">` |
| Métricas (200%, 550K...) | `.stat-num` |
| Bio/descrição | `data-en="..."` e `data-pt="..."` nos elementos |
| Experiências | seção `#about-card` |
| Links (LinkedIn, Behance) | `href="..."` nos elementos `contact-link` |
| Contato (email, tel) | seção `#contact-card` |
| Cores do site | variáveis CSS em `:root { ... }` |

**Para editar online (sem instalar nada):**
- No GitHub, clique no arquivo `index.html` → clique no lápis ✏️ → edite → "Commit changes"

**Editor recomendado (gratuito):**
- **VS Code** (code.visualstudio.com) — melhor experiência de edição

---

## 🤖 Melhor IA para criar/evoluir o site

| Ferramenta | Para que usar | Preço |
|---|---|---|
| **Claude.ai** (este!) | Gerar/editar HTML completo, adicionar seções, melhorar copy | Grátis (limitado) / $20/mês |
| **Cursor** | Editor de código com IA integrada, perfeito para editar o site | Grátis (limitado) |
| **v0.dev** (Vercel) | Gerar componentes novos em React/HTML | Grátis (limitado) |
| **Framer AI** | Site com IA, mas menos customizável | Grátis (com marca d'água) |

**Prompt modelo para pedir melhorias ao Claude:**
```
Tenho um portfólio HTML de product designer com tema de mapa do tesouro.
Quero [adicionar uma seção de X / mudar a cor Y / adicionar animação Z].
Aqui está o HTML atual: [cole o conteúdo do index.html]
```

---

## 🎮 Como navegar no site (para visitantes)

| Ação | Resultado |
|---|---|
| Scroll para baixo / seta → | Próxima ilha |
| Scroll para cima / seta ← | Ilha anterior |
| Clicar nos pontos (barra inferior) | Ir para ilha específica |
| Clicar no menu superior | Navegar por seção |
| Arrastar no touchscreen | Navegar (swipe) |
| Clicar "Read case →" | Abrir case study completo |
| Tecla ESC | Fechar case study |
| Toggle EN/PT | Mudar idioma |

---

## 📊 Desempenho esperado

- **Tamanho**: ~15KB HTML + imagens (carregamento rápido)
- **Mobile**: layout adaptado automaticamente (vertical scroll)
- **SEO**: meta tags básicas incluídas
- **Acessibilidade**: navegação por teclado funcional

---

## 🔮 Próximos passos sugeridos

1. **Adicionar Google Analytics** (grátis): colar script antes do `</head>`
2. **Adicionar segundo case study** quando disponível
3. **Adicionar CV para download**: `<a href="assets/CV_Jose_Araujo.pdf" download>`
4. **Compressor de imagens**: use tinypng.com antes de subir as imagens (mantém qualidade, reduz tamanho)

---

*Qualquer dúvida no processo, peça ajuda ao Claude: cole este README + o arquivo index.html e descreva o que precisa.*
