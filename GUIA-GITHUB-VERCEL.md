# 📚 Guia Completo: GitHub + Vercel para seu Dashboard

## Passo 1: Criar Conta no GitHub (se não tiver)

1. Acesse: **github.com**
2. Clique em **"Sign up"**
3. Preencha email, senha e nome de usuário
4. Confirme o email
5. **Pronto!** Você tem sua conta GitHub

---

## Passo 2: Criar Repositório no GitHub

1. No seu GitHub, clique em **"+"** (canto superior direito)
2. Clique em **"New repository"**
3. Preencha:
   - **Repository name**: `dashboard-equipe-5605`
   - **Description**: `Dashboard interativo para reunião semanal de casos clínicos`
   - **Visibility**: Escolha **"Private"** (privado, só você acessa) ou **"Public"** (qualquer um vê)
   - ✅ Marque **"Add a README file"** (já tem pronto!)
4. Clique em **"Create repository"**

**Você agora tem um repositório vazio no GitHub.**

---

## Passo 3: Fazer Upload dos Arquivos no GitHub

### Opção A: Via GitHub Web (mais fácil, sem instalar nada)

1. No seu repositório, clique em **"Add file"** → **"Upload files"**
2. Clique em **"choose your files"** ou arraste os arquivos
3. **Selecione estes arquivos** da pasta que preparei:
   - `index.html` (o dashboard principal v16)
   - `README.md`
   - `.gitignore`
   - `claude_roteiro_forms_acs.md` (para referência)
   - Todas as versões anteriores (v15, v14, v13, v12.1)

4. Em **"Commit message"**, escreva:
   ```
   Upload do dashboard v16 e versões anteriores
   ```

5. Clique em **"Commit changes"**

**Pronto! Seus arquivos estão no GitHub.**

---

### Opção B: Via Git no Computador (mais profissional)

Se quiser aprender a usar Git (recomendo para atualizações futuras):

1. **Instale Git**: git-scm.com
2. **Abra o Terminal/Prompt de Comando** na pasta dos arquivos
3. Execute:

```bash
git init
git add .
git commit -m "Upload do dashboard v16 e versões anteriores"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/dashboard-equipe-5605.git
git push -u origin main
```

(Troque `SEU-USUARIO` pelo seu nome de usuário do GitHub)

---

## Passo 4: Conectar na Vercel e Deploy

### Vercel vai se conectar com GitHub e fazer deploy automaticamente

1. Acesse: **vercel.com**
2. Clique em **"Sign up"**
3. Escolha **"Continue with GitHub"**
4. Autorize o Vercel a acessar sua conta GitHub
5. Clique em **"New Project"**
6. Procure seu repositório **"dashboard-equipe-5605"** e clique nele
7. Vercel vai detectar que é um HTML estático (não precisa configurar nada!)
8. Clique em **"Deploy"**

**⏳ Aguarde 1-2 minutos...**

---

## 🎉 Pronto!

Você receberá uma **URL** como:
```
https://dashboard-equipe-5605.vercel.app
```

**Essa é sua URL para acessar o dashboard de qualquer lugar!**

---

## 🔄 Como Atualizar o Dashboard

Sempre que quiser atualizar (melhorias, correções, nova versão):

### Opção A: Via GitHub Web
1. Abra o arquivo no GitHub
2. Clique no ✏️ (editar)
3. Faça as mudanças
4. Clique em **"Commit changes"**
5. **Vercel atualiza automaticamente em 1-2 minutos**

### Opção B: Via Git (se instalou)
```bash
# Faça suas mudanças nos arquivos locais, depois:
git add .
git commit -m "Descrição da mudança"
git push
```

---

## 💡 Dicas

- **Versão sempre atualizada**: Qualquer pessoa que acessar `dashboard-equipe-5605.vercel.app` vê a versão mais recente
- **Histórico completo**: GitHub mantém todas as versões anteriores (pode voltar se errar)
- **Não precisa de senhas**: Vercel acessa direto do GitHub
- **Pode compartilhar**: Mande o link para qualquer pessoa acessar (se for repositório público)
- **Mobile funciona**: Dashboard funciona perfeitamente em celular e tablet

---

## ❓ Dúvidas?

**Precisa voltar para uma versão anterior?**
- GitHub → Seu repositório → Clique em versão anterior → Restaurar
- Vercel atualiza automaticamente

**Quer fazer mais seguro (não público)?**
- Crie o repositório como **"Private"**
- Vercel continua funcionando igual

**Quer adicionar senha?**
- Avançado: Vercel oferece proteção com password nos planos pagos
- Básico: Mande o link só para quem precisa

---

## 📞 Próximos Passos (Opcional)

Depois de tudo funcionando, podemos:
- ✅ Automatizar importação do Forms (sem precisar baixar Excel)
- ✅ Notificações automáticas quando novo caso entra
- ✅ Integração com Google Drive para histórico
- ✅ Relatórios mensais automáticos

Mas por agora, foco em colocar no ar! 🚀

---

**Você consegue! Qualquer dúvida neste guia, avise.**
