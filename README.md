# ☕ estouemreuniao.com.br

Simulador de reunião realista pra parecer ocupadíssimo e evitar interrupções.

## 🚀 Como subir no ar (passo a passo)

### 1. Configure suas informações no `index.html`

No início do `<script>`, edite as duas linhas:

```js
const PIX_KEY = 'SEU_EMAIL@pix.com';       // sua chave Pix (email, CPF, telefone, etc)
const BMC_URL = 'https://buymeacoffee.com/SEU_USUARIO'; // seu perfil no Buy Me a Coffee
```

Também procure a div `#qr-img` e substitua pelo seu QR Code Pix:
```html
<div class="qr-placeholder" id="qr-img">
  <img src="qrcode-pix.png" alt="QR Code Pix" style="width:100%;border-radius:8px;" />
</div>
```

---

### 2. Crie o repositório no GitHub

```bash
git init
git add .
git commit -m "🚀 primeiro commit"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/estouemreuniao.git
git push -u origin main
```

---

### 3. Deploy no Vercel (gratuito)

1. Acesse [vercel.com](https://vercel.com) e faça login com o GitHub
2. Clique em **Add New Project**
3. Importe o repositório `estouemreuniao`
4. Clique em **Deploy** — pronto, já está no ar em ~30s
5. Você recebe uma URL do tipo `estouemreuniao.vercel.app`

---

### 4. Compre o domínio

**Opção 1 — Registro.br** (domínio .com.br, ~R$40/ano):
- Acesse [registro.br](https://registro.br)
- Busque `estouemreuniao.com.br`
- Compre e anote os nameservers

**Opção 2 — Namecheap** (domínio .com, ~$10/ano):
- Acesse [namecheap.com](https://namecheap.com)

---

### 5. Conecte o domínio ao Vercel

1. No painel do Vercel, vá em **Settings → Domains**
2. Adicione `estouemreuniao.com.br`
3. O Vercel vai te dar um registro DNS pra adicionar
4. Vá ao painel do Registro.br e adicione o registro CNAME/A indicado
5. Aguarde ~10 minutos para propagar

---

### 6. Configure o Buy Me a Coffee (opcional)

1. Acesse [buymeacoffee.com](https://buymeacoffee.com) e crie uma conta gratuita
2. Personalize sua página
3. Copie a URL do seu perfil e coloque no `BMC_URL` do código

---

## 💡 Melhorias futuras

- [ ] Adicionar mais tipos de reunião
- [ ] Modo "emergência" com atalho de teclado
- [ ] Sons de reunião (notificações, digitação)
- [ ] Compartilhar link da "reunião" pra trollar amigos
- [ ] PWA para instalar no celular

---

Feito com ☕ — se usar, me manda um Pix!
