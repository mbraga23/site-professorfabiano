# Site Institucional - Vereador [NOME]

Site de uma página com navegação por abas, responsivo e pronto para hospedar no GitHub Pages.

---

## 📋 O que você precisa fazer

### 1. Personalizar o conteúdo

Abra o arquivo `index.html` e substitua os textos entre colchetes:

- `[NOME]` → Nome do vereador
- `[NOME COMPLETO]` → Nome completo
- `[CIDADE]` → Cidade
- `[DATA DE NASCIMENTO]` → Data de nascimento
- `[CÔNJUGE]` → Nome do cônjuge
- `[ANO]` → Ano da eleição
- `[ESCOLA]` → Escola onde estudou
- `[GRADUAÇÃO]` → Curso superior (se tiver)
- `[INSTITUIÇÃO]` → Universidade/faculdade
- E os demais campos...

### 2. Trocar as fotos

Substitua as URLs de placeholder pelas fotos reais. Exemplo:

```html
<!-- ANTES -->
<img src="https://via.placeholder.com/300x350/1a365d/ffffff?text=Foto+Oficial" alt="Foto oficial">

<!-- DEPOIS -->
<img src="fotos/foto-oficial.jpg" alt="Foto oficial do Vereador Fulano">
```

Crie uma pasta `fotos/` no repositório e coloque as imagens lá.

### 3. Configurar o formulário de contato (Formspree)

O formulário usa o **Formspree** (gratuito para até 50 envios/mês):

1. Acesse [formspree.io](https://formspree.io) e crie uma conta grátis
2. Clique em **"New Form"**
3. Dê um nome (ex: "Contato Vereador")
4. Copie o ID do formulário (aparece na URL, ex: `xyzabcde`)
5. No `index.html`, substitua `YOUR_FORM_ID` pelo ID:

```html
<!-- ANTES -->
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">

<!-- DEPOIS -->
<form action="https://formspree.io/f/xyzabcde" method="POST">
```

As mensagens cairão direto no email cadastrado no Formspree!

---

## 🚀 Como hospedar no GitHub Pages

### Passo a passo:

1. **Crie uma conta no GitHub** (se não tiver): [github.com](https://github.com)

2. **Crie um novo repositório:**
   - Clique no "+" no canto superior direito → "New repository"
   - Nome: `vereador-fulano` (ou outro nome)
   - Deixe como **Public**
   - Clique em "Create repository"

3. **Faça upload dos arquivos:**
   - Na página do repositório, clique em "uploading an existing file"
   - Arraste o `index.html` e a pasta `fotos/` (se tiver)
   - Escreva uma mensagem de commit (ex: "Site inicial")
   - Clique em "Commit changes"

4. **Ative o GitHub Pages:**
   - Vá em **Settings** (configurações do repositório)
   - No menu lateral, clique em **Pages**
   - Em "Source", selecione **Deploy from a branch**
   - Em "Branch", selecione **main** e **/ (root)**
   - Clique em **Save**

5. **Aguarde ~1 minuto** e acesse seu site:
   ```
   https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/
   ```

---

## 🎨 Personalizações opcionais

### Mudar as cores

No início do CSS, altere as variáveis:

```css
:root {
    --azul-escuro: #1a365d;    /* Cor principal */
    --azul-medio: #2c5282;     /* Cor secundária */
    --dourado: #d69e2e;        /* Destaques */
}
```

### Adicionar redes sociais

Adicione links no footer ou na seção de contato.

### Domínio personalizado

Se o cliente tiver um domínio (ex: `www.vereadorfunalo.com.br`):

1. No GitHub Pages, em "Custom domain", digite o domínio
2. No provedor de domínio, configure o DNS apontando para o GitHub

---

## 📁 Estrutura de arquivos

```
📂 repositório/
├── 📄 index.html      (o site)
├── 📄 README.md       (este arquivo)
└── 📂 fotos/          (pasta de imagens)
    ├── foto-oficial.jpg
    ├── atuacao.jpg
    └── ...
```

---

## ✅ Checklist antes de publicar

- [ ] Substituí todos os `[TEXTOS]` placeholder
- [ ] Coloquei as fotos reais
- [ ] Configurei o Formspree com o ID correto
- [ ] Testei o formulário de contato
- [ ] Verifiquei no celular (responsivo)
- [ ] Ativei o GitHub Pages

---

**Pronto!** Site no ar com custo ZERO. 🎉
