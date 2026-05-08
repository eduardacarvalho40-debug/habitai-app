# HabitAI 💙✨

App de rastreamento de hábitos com IA.

---

## Como publicar (passo a passo)

### 1. Criar repositório no GitHub

1. Acesse [github.com](https://github.com) e faça login
2. Clique no **+** no canto superior direito → **New repository**
3. Nome sugerido: `habitai-app`
4. Deixe como **Public**
5. Clique em **Create repository**
6. Faça upload dos arquivos desta pasta:
   - Clique em **uploading an existing file**
   - Arraste todos os arquivos e a pasta `api/`
   - Clique em **Commit changes**

---

### 2. Pegar sua chave da API Anthropic

1. Acesse [console.anthropic.com](https://console.anthropic.com)
2. Vá em **API Keys** no menu lateral
3. Clique em **Create Key**
4. Copie a chave (começa com `sk-ant-...`) — guarde em lugar seguro

---

### 3. Publicar no Vercel

1. Acesse [vercel.com](https://vercel.com) e clique em **Sign Up with GitHub**
2. Na tela inicial, clique em **Add New Project**
3. Encontre o repositório `habitai-app` e clique em **Import**
4. Na tela de configuração, **antes de clicar em Deploy**:
   - Abra a seção **Environment Variables**
   - Nome: `ANTHROPIC_API_KEY`
   - Valor: cole sua chave `sk-ant-...`
   - Clique em **Add**
5. Clique em **Deploy**
6. Aguarde ~1 minuto e pronto! 🎉

O Vercel vai te dar um link tipo:
`https://habitai-app.vercel.app`

---

### 4. Atualizar o app no futuro

Sempre que quiser mudar algo:
1. Edite os arquivos no GitHub (botão do lápis)
2. Salve (Commit changes)
3. O Vercel republica automaticamente em ~30 segundos

---

## Estrutura do projeto

```
habitai-app/
├── index.html        ← O app completo (visual + lógica)
├── api/
│   └── chat.js       ← Servidor que chama a API Anthropic
├── vercel.json       ← Configuração do Vercel
└── README.md         ← Este arquivo
```

---

Feito com 💙 usando Claude + Vercel
