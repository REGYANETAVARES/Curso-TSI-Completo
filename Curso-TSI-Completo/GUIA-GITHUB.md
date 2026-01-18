# 🚀 GUIA: Como Subir Este Repositório para o GitHub

## 📋 **Passo a Passo Completo**

### **OPÇÃO 1: Criar Repositório Novo no GitHub** (Recomendado)

#### **Passo 1: Criar Repositório no GitHub**
1. Acesse [github.com](https://github.com)
2. Clique no **+** (canto superior direito) → **New repository**
3. Configure:
   - **Nome:** `Curso-TSI-Completo`
   - **Descrição:** `Material completo do curso de TSI - IF Goiano`
   - **Visibilidade:** Public ✅
   - **NÃO** marque "Initialize with README" (já temos um)
4. Clique em **Create repository**

#### **Passo 2: Subir os Arquivos**

**Via GitHub Website (Mais Fácil):**
1. No repositório criado, clique em **uploading an existing file**
2. Arraste TODA a pasta `Curso-TSI-Completo` para lá
3. Escreva uma mensagem: `🎓 Adicionar material completo do curso TSI`
4. Clique em **Commit changes**

**Via Git (Linha de Comando):**
```bash
# Navegar até a pasta
cd caminho/para/Curso-TSI-Completo

# Inicializar git
git init

# Adicionar todos os arquivos
git add .

# Fazer commit
git commit -m "🎓 Adicionar material completo do curso TSI"

# Conectar ao GitHub (substitua SEU-USUARIO)
git remote add origin https://github.com/REGYANETAVARES/Curso-TSI-Completo.git

# Subir os arquivos
git branch -M main
git push -u origin main
```

---

### **OPÇÃO 2: Adicionar ao Repositório Existente**

Se você já tem um repositório e quer adicionar este material:

```bash
# Copiar arquivos para seu repositório existente
cp -r Curso-TSI-Completo/* /caminho/do/seu/repositorio/

# Ir para o repositório
cd /caminho/do/seu/repositorio/

# Adicionar novos arquivos
git add .

# Commit
git commit -m "🎓 Adicionar material organizado do curso TSI"

# Subir
git push
```

---

## 📦 **Estrutura Que Será Criada no GitHub**

```
REGYANETAVARES/Curso-TSI-Completo/
│
├── .gitignore
├── README.md ⭐ (Página principal do repositório)
│
├── 1-Periodo/
│   └── Algoritmos-Programacao/
│       ├── README.md
│       ├── aulas-transcritas/ (6 PDFs)
│       ├── exercicios/
│       └── codigos/
│
└── 3-Periodo/
    ├── Modelagem-Sistemas-UML/
    │   ├── README.md
    │   ├── aulas-transcritas/ (7 DOCXs)
    │   ├── diagramas/
    │   └── exercicios/
    │
    └── POO/
        ├── README.md
        ├── aulas-transcritas/ (9 arquivos)
        ├── exercicios/
        └── projetos/
```

---

## 🎨 **Customizações Recomendadas**

### **1. Adicionar Badge no README Principal**

Abra o `README.md` principal e adicione no topo:

```markdown
<div align="center">

![GitHub stars](https://img.shields.io/github/stars/REGYANETAVARES/Curso-TSI-Completo?style=social)
![GitHub forks](https://img.shields.io/github/forks/REGYANETAVARES/Curso-TSI-Completo?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/REGYANETAVARES/Curso-TSI-Completo?style=social)

</div>
```

### **2. Adicionar Imagem de Capa**

Crie uma imagem bonita (Canva, Figma) e adicione:
- Salve como `capa.png` na raiz
- Adicione no README: `![Capa](./capa.png)`

### **3. Adicionar Topics no GitHub**

Na página do repositório:
- Clique em ⚙️ (Settings) → Topics
- Adicione: `tsi`, `educacao`, `if-goiano`, `programacao`, `java`, `uml`, `poo`

---

## 🔗 **Após Subir, Você Pode:**

### **Compartilhar:**
- Link direto: `https://github.com/REGYANETAVARES/Curso-TSI-Completo`
- No LinkedIn
- No currículo
- Com colegas de classe

### **Fixar no Perfil:**
1. Vá no seu perfil do GitHub
2. Clique em "Customize your pins"
3. Selecione este repositório

### **Adicionar ao README do seu Perfil:**
```markdown
## 📚 Repositórios em Destaque

- [🎓 Curso TSI Completo](https://github.com/REGYANETAVARES/Curso-TSI-Completo) - Material organizado do curso de TSI
```

---

## 📈 **Manutenção do Repositório**

### **Adicionar Novo Conteúdo:**
```bash
# Adicionar novos arquivos
git add .
git commit -m "📝 Adicionar aulas do 2º período"
git push
```

### **Atualizar README:**
```bash
git add README.md
git commit -m "📝 Atualizar documentação"
git push
```

---

## ✨ **Próximos Passos Sugeridos**

1. ✅ Subir o repositório
2. ✅ Adicionar topics no GitHub
3. ✅ Compartilhar no LinkedIn
4. ⏳ Adicionar material do 2º período
5. ⏳ Criar projetos práticos
6. ⏳ Adicionar exercícios resolvidos

---

## 🆘 **Problemas Comuns**

### **Erro: "Repository already exists"**
- Escolha outro nome ou delete o repositório existente

### **Erro ao fazer push**
```bash
# Configure seu usuário do git
git config --global user.email "seu-email@gmail.com"
git config --global user.name "Seu Nome"
```

### **Arquivo muito grande**
- GitHub tem limite de 100MB por arquivo
- Comprima ou divida arquivos grandes

---

## 🎯 **Resultado Final**

Seu repositório ficará PROFISSIONAL:
- ✅ Organizado por períodos
- ✅ READMEs completos e informativos
- ✅ Fácil navegação
- ✅ Pronto para compartilhar
- ✅ Impressiona recrutadores

---

## 💡 **Dica Extra**

Depois de subir, tire um print da página do GitHub e adicione no seu portfólio/currículo!

---

<div align="center">

**🚀 Bora pro GitHub!**

Qualquer dúvida, consulte a [documentação oficial do GitHub](https://docs.github.com)

</div>
