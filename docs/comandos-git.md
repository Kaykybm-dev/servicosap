# 📚 Minha Cola de Git — ServiçosAP
> Feito por Kayky | Engenheiro Sênior: Eko

---

## ⚙️ Configuração Inicial (faz só uma vez)

```bash
# Configurar seu nome
git config --global user.name "Kayky"

# Configurar seu email (mesmo do GitHub)
git config --global user.email "seu-email@gmail.com"

# Definir branch padrão como main
git config --global init.defaultBranch main

# Verificar se tudo foi salvo
git config --global --list
```

---

## 🚀 Começando um Projeto

```bash
# Inicializar o Git na pasta do projeto
git init

# Clonar um projeto do GitHub para sua máquina
git clone https://github.com/usuario/repositorio.git
```

---

## 📸 O Ciclo de Vida do Dia a Dia

```
Você edita arquivos
      ↓
git add (seleciona o que vai fotografar)
      ↓
git commit (tira a fotografia com mensagem)
      ↓
git push (envia para o GitHub)
```

```bash
# Ver o que mudou no projeto (USE SEMPRE!)
git status

# Adicionar um arquivo específico
git add index.html

# Adicionar TUDO de uma vez
git add .

# Tirar a fotografia com mensagem
git commit -m "Mensagem descrevendo o que foi feito"

# Enviar para o GitHub
git push origin main

# Baixar atualizações do GitHub
git pull origin main
```

---

## 🌿 Branches (Galhos)

```bash
# Ver em qual branch você está
git branch

# Criar uma nova branch
git branch feature/nome-da-feature

# Mudar para uma branch
git checkout nome-da-branch

# Criar E já mudar para ela (atalho)
git checkout -b feature/nome-da-feature

# Voltar para a main
git checkout main

# Mesclar uma branch na main (estando na main)
git merge feature/nome-da-feature
```

### Exemplos de nomes de branch:
```
feature/cadastro-prestador
feature/pagina-busca
fix/botao-quebrado
docs/atualiza-readme
```

---

## 📜 Histórico

```bash
# Ver histórico de commits completo
git log

# Ver histórico resumido (mais útil)
git log --oneline
```

---

## ✍️ Regras de Ouro para Mensagens de Commit

**Teste mental:** "Se aplicado, este commit vai..."

| ✅ Bom | ❌ Ruim |
|--------|---------|
| `Adiciona formulário de cadastro` | `arrumei` |
| `Corrige bug na validação de email` | `mudanças` |
| `Cria rota de busca por categoria` | `commit` |
| `Atualiza README com instruções` | `asdfsdf` |

### Regras:
- Verbo no presente
- Seja específico
- Sem acento (boa prática)
- Máximo ~72 caracteres

---

## 🔗 Conectando ao GitHub

```bash
# Adicionar o repositório remoto
git remote add origin https://github.com/SEU-USERNAME/servicosap.git

# Verificar se foi adicionado
git remote -v

# Primeiro push (sobe a branch main)
git push -u origin main

# Pushs seguintes (mais simples)
git push
```

---

## 🆘 Comandos de Emergência

```bash
# Desfazer mudanças em um arquivo antes do add
git checkout -- nome-do-arquivo.html

# Remover um arquivo do add (antes do commit)
git reset HEAD nome-do-arquivo.html

# Ver diferença do que mudou
git diff
```

---

## 📁 Estrutura do ServiçosAP

```
servicosap/
├── frontend/     ← HTML, CSS, JavaScript
├── backend/      ← Python + FastAPI
├── docs/         ← Documentos do projeto
└── README.md     ← Apresentação do projeto
```

---

> 💡 **Lembra:** No terminal, silêncio = sucesso!
> 💡 **Lembra:** `git status` é seu melhor amigo, use sempre!
