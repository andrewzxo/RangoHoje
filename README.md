# 🍲 RangoHoje | ETEC Dr. Carolino da Motta e Silva

> Plataforma inteligente para consulta do cardápio da merenda escolar, tabela nutricional de cada ingrediente, filaômetro colaborativo e mural da comunidade para os alunos da **ETEC Dr. Carolino da Motta e Silva** (Centro Paula Souza / Governo de SP).

---

## 🚀 Como Subir para o GitHub

1. Abra o terminal nesta pasta (ou no VS Code / Antigravity):
```bash
git init
git add .
git commit -m "feat: site da merenda RangoHoje - ETEC Dr. Carolino da Motta e Silva"
```

2. Crie um novo repositório no seu GitHub (público ou privado).
3. Conecte o repositório e envie os arquivos:
```bash
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/NOME-DO-REPOSITORIO.git
git push -u origin main
```

---

## ☁️ Como Fazer Deploy Gratuito no Cloudflare Pages

O Cloudflare Pages oferece **hospedagem 100% gratuita, sem limite de visitas e com SSL (HTTPS) automático**.

### Método Recomendado (Via GitHub com deploy automático a cada alteração):
1. Acesse o painel do [Cloudflare Dashboard](https://dash.cloudflare.com/) e vá em **Workers & Pages**.
2. Clique em **Create application** > **Pages** > **Connect to Git**.
3. Selecione o repositório que você acabou de subir no GitHub.
4. Preencha as configurações de build:
   - **Framework preset:** `Vite`
   - **Build command:** `npm run build`
   - **Build output directory:** `dist`
   - **Root directory:** `/` (deixe em branco se o repositório estiver na raiz)
5. Clique em **Save and Deploy**. Em menos de 1 minuto, seu site estará no ar com link público (ex: `rango-hoje-etec.pages.dev`).

### Método Direto (Arrastar a pasta `dist` sem precisar de Git):
1. No Cloudflare Pages, escolha **Upload assets**.
2. Dê um nome ao projeto (ex: `rango-etec`).
3. Arraste a pasta `dist` gerada pelo comando `npm run build`.
4. Pronto! O site entra no ar instantaneamente.

---

## 🔒 Informações de Acesso (Apresentação)

- **Painel das Merendeiras:** O botão de acesso fica no topo e na barra flutuante mobile.
- **PIN Padrão de Apresentação:** `1234`
- *Observação de Segurança:* A senha NÃO é exibida em nenhuma tela para garantir que apenas pessoas autorizadas tenham acesso.

---

## 🛠️ Tecnologias Utilizadas

- **React 19 + TypeScript**
- **Vite 8 + `@tailwindcss/vite`**
- **Tailwind CSS v4**
- **Lucide Icons**
- **Canvas-Confetti**
- **LocalStorage API** (zero dependência de banco de dados pago)
