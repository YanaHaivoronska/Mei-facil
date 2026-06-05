# MEI Fácil 📱

App de controle financeiro e declaração de imposto para Microempreendedor Individual (MEI), funciona como PWA instalável no celular.

## Funcionalidades

- ✅ Lançamento de receitas e despesas
- 📷 Foto de cheques e comprovantes
- 📊 Gráficos mensais de receitas, despesas e lucro
- 🧾 Cálculo automático para DASN-SIMEI
- 📉 Base tributável IRPF (8% comércio / 32% serviços)
- ⏰ Lembretes de vencimento do DAS-MEI
- 📤 Exportação CSV (Excel) e relatório HTML
- 📲 Instalável no celular (PWA)
- 🌙 Modo escuro automático
- ✈️ Funciona offline

---

## Como publicar no GitHub Pages

### 1. Crie um repositório no GitHub
- Acesse [github.com](https://github.com) e faça login
- Clique em **"New repository"**
- Nome sugerido: `mei-facil`
- Deixe como **Public**
- Clique em **"Create repository"**

### 2. Faça upload dos arquivos
Você tem duas opções:

**Opção A — pelo site (mais fácil):**
- Na página do repositório clique em **"uploading an existing file"**
- Arraste os 3 arquivos: `index.html`, `manifest.json`, `sw.js`
- Clique em **"Commit changes"**

**Opção B — pelo terminal (Git):**
```bash
git init
git add .
git commit -m "MEI Fácil - primeiro deploy"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/mei-facil.git
git push -u origin main
```

### 3. Ative o GitHub Pages
- No repositório, clique em **Settings** (engrenagem)
- No menu lateral esquerdo, clique em **Pages**
- Em **"Branch"**, selecione `main` e pasta `/ (root)`
- Clique em **Save**

### 4. Acesse o app
Após 1-2 minutos seu app estará disponível em:
```
https://SEU_USUARIO.github.io/mei-facil/
```

### 5. Instale no celular
- **Android:** Abra o link no Chrome → menu (⋮) → "Adicionar à tela inicial"
- **iPhone:** Abra no Safari → botão Compartilhar → "Adicionar à Tela de Início"

---

## Estrutura dos arquivos

```
mei-facil/
├── index.html      ← App principal
├── manifest.json   ← Configuração PWA
├── sw.js           ← Service Worker (modo offline)
└── README.md       ← Este arquivo
```

## Ícones (opcional)

Para ter ícone personalizado no celular, adicione:
- `icon-192.png` — 192×192 pixels
- `icon-512.png` — 512×512 pixels

Se não adicionar, o navegador usará um ícone padrão.

---

## Observações

- Os dados ficam salvos no `localStorage` do navegador (no próprio celular)
- Para não perder os dados, não limpe o cache do navegador
- O relatório exportado é um arquivo `.html` que pode ser aberto no navegador e impresso como PDF

---

Desenvolvido com ❤️ para MEIs brasileiros.
