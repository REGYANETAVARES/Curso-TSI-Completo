# 📗 Modelagem de Sistemas (UML)

> **3º Período**  
> Diagramas de Caso de Uso, Requisitos e Modelagem de Sistemas

---

## 📋 **Sobre a Disciplina**

Disciplina focada em modelagem de sistemas utilizando UML (Unified Modeling Language), com ênfase em Diagramas de Caso de Uso, análise de requisitos, regras de negócio e especificação de sistemas.

**Ferramenta Principal:** StarUML

---

## 🎯 **Objetivos de Aprendizado**

- Compreender e criar Diagramas de Caso de Uso
- Identificar atores e casos de uso em sistemas
- Aplicar relacionamentos: Associação, Include, Extend, Herança
- Diferenciar requisitos funcionais de regras de negócio
- Especificar casos de uso textualmente
- Modelar sistemas completos

---

## 📚 **Conteúdo Programático**

### **Módulo 1: Fundamentos de Casos de Uso**
- O que são atores
- O que são casos de uso
- Associação simples
- Identificação de funcionalidades

### **Módulo 2: Relacionamentos**
- **Include:** Relacionamento obrigatório
- **Extend:** Relacionamento opcional
- **Herança:** Generalização/Especialização
- Quando usar cada tipo

### **Módulo 3: Requisitos e Regras de Negócio**
- Requisitos funcionais
- Requisitos não-funcionais
- Regras de negócio
- Desempenho e segurança

### **Módulo 4: Especificação Textual**
- Estrutura de um caso de uso textual
- Pré-condições e pós-condições
- Fluxo básico
- Fluxos alternativos

---

## 📂 **Estrutura de Arquivos**

```
Modelagem-Sistemas-UML/
├── README.md (este arquivo)
├── aulas-transcritas/
│   ├── 01-casos-de-uso.docx
│   ├── 02-heranca-permissoes.docx
│   ├── 03-extend.docx
│   ├── 04-atributos-vs-casos-uso.docx
│   ├── 05-include.docx
│   ├── 06-requisitos-regras-negocio.docx
│   └── 07-especificacao-textual.docx
├── diagramas/
│   └── (diagramas a serem adicionados)
└── exercicios/
    └── (exercícios a serem adicionados)
```

---

## 🎓 **Aulas Disponíveis**

### **Aula 1: Introdução a Casos de Uso**
- Conceito de atores (usuários, hardware, sistemas externos)
- Conceito de casos de uso (funcionalidades)
- Associação simples (ator ↔ caso de uso)
- Ferramenta StarUML

### **Aula 2: Herança e Permissões**
- Herança entre atores
- Exemplo: Funcionário → Gerente → Administrador
- Especialização vs Generalização
- Controle de permissões

### **Aula 3: Relacionamento Extend**
- Conceito de extensão opcional
- Quando usar extend
- Exemplos práticos: tanque cheio, motorista adicional
- Diferença entre extend e include

### **Aula 4: Atributos vs Casos de Uso**
- O que NÃO é caso de uso (atributos)
- Casos de uso são ações (verbos)
- Atributos vão no texto descritivo
- Exemplo: "dia" e "sala" são atributos, não casos de uso

### **Aula 5: Relacionamento Include**
- Conceito de inclusão obrigatória
- Reuso de funcionalidades
- Exemplo: "Identificar Cliente" usado por múltiplos casos de uso
- Quando usar include

### **Aula 6: Requisitos e Regras de Negócio**
- Requisitos funcionais vs não-funcionais
- Regras de negócio
- Desempenho, segurança, usabilidade
- Documentação associada

### **Aula 7: Especificação Textual**
- Estrutura completa de um caso de uso
- Pré-condições e pós-condições
- Fluxo básico e alternativos
- Exemplo completo: Venda de Ingressos

---

## 💡 **Conceitos-Chave**

### **Elementos de um Diagrama de Caso de Uso**

| Elemento | Descrição | Representação |
|----------|-----------|---------------|
| **Ator** | Usuário ou sistema externo | 🧑 Boneco palito |
| **Caso de Uso** | Funcionalidade do sistema | ⭕ Elipse |
| **Associação** | Ligação ator-caso de uso | ― Linha simples |
| **Include** | Relação obrigatória | ← - - ‹‹include›› |
| **Extend** | Relação opcional | ← - - ‹‹extend›› |
| **Herança** | Generalização | △ Triângulo |

### **Relacionamentos: Quando Usar**

```
ASSOCIAÇÃO SIMPLES:
- Entre ator e caso de uso
- Define quem tem acesso à funcionalidade

INCLUDE (obrigatório):
- Um caso de uso sempre precisa de outro
- Exemplo: "Efetuar Venda" INCLUDE "Identificar Cliente"

EXTEND (opcional):
- Um caso de uso opcionalmente aciona outro
- Exemplo: "Registrar Sessão" EXTEND "Criar Promoção"

HERANÇA:
- Entre atores: especialização de permissões
- Entre casos de uso: generalização de funcionalidades
```

---

## 🎯 **Exemplos Práticos**

### **Exemplo 1: Sistema de Cinema**

**Atores:**
- Cliente
- Funcionário
- Gerente
- Administrador

**Casos de Uso:**
- Comprar Ingresso
- Cadastrar Filme
- Cadastrar Sessão
- Gerar Relatório
- Criar Promoção
- Gerenciar Usuários

**Relacionamentos:**
- Cliente → Comprar Ingresso (associação)
- Gerente herda de Funcionário
- Administrador herda de Gerente
- Comprar Ingresso INCLUDE Identificar Cliente
- Cadastrar Sessão EXTEND Criar Promoção

### **Exemplo 2: Sistema de Locadora**

**Casos de Uso:**
- Alocar Veículo
  - EXTEND: Solicitar Tanque Cheio
  - EXTEND: Adicionar Motorista

---

## 📖 **Especificação Textual de Caso de Uso**

### **Template Padrão:**

```
NOME: <Nome do Caso de Uso>
ATOR: <Ator principal>
PRÉ-CONDIÇÕES: <O que deve existir antes>
PÓS-CONDIÇÕES: <O que muda após a execução>

FLUXO BÁSICO:
1. O ator faz X
2. O sistema faz Y
3. O ator informa Z
4. O sistema calcula W
5. Fim do caso de uso

FLUXOS ALTERNATIVOS:
A1: <Exceção 1>
1. Se condição X
2. O sistema faz Y
3. Retorna ao passo N do fluxo básico

REGRAS DE NEGÓCIO:
RN01: <Descrição da regra>
RN02: <Descrição da regra>
```

### **Exemplo Completo: Vender Ingresso**

```
NOME: Vender Ingresso
ATOR: Funcionário, Cliente
PRÉ-CONDIÇÕES: 
- Filme cadastrado
- Sessão cadastrada
- Poltronas disponíveis

PÓS-CONDIÇÕES:
- Bilhete vendido
- Poltrona reservada
- Pagamento registrado

FLUXO BÁSICO:
1. O funcionário seleciona o filme
2. O sistema apresenta as sessões disponíveis
3. O funcionário seleciona a sessão
4. O sistema apresenta as poltronas disponíveis
5. O funcionário seleciona a poltrona
6. O sistema calcula o valor
7. O funcionário registra o pagamento
8. O sistema gera o bilhete
9. Fim do caso de uso

FLUXOS ALTERNATIVOS:
A1: Aplicar Promoção
1. No passo 6, se houver promoção ativa
2. O sistema aplica o desconto
3. Retorna ao passo 7

A2: Poltrona Indisponível
1. No passo 5, se poltrona já estiver reservada
2. O sistema informa ao funcionário
3. Retorna ao passo 4

REGRAS DE NEGÓCIO:
RN01: Poltrona deve ser bloqueada imediatamente após seleção
RN02: Desconto de promoção não cumulativo
RN03: Bilhete só é gerado após confirmação de pagamento
```

---

## 🛠️ **Ferramentas**

### **StarUML**
- Ferramenta principal da disciplina
- Criar diagramas profissionais
- Exportar em diversos formatos

### **Alternativas:**
- Lucidchart
- Draw.io
- Visual Paradigm
- PlantUML (código)

---

## ✍️ **Exercícios Recomendados**

1. **Básico:**
   - Criar diagrama para sistema de biblioteca
   - Identificar 3 atores e 5 casos de uso
   - Usar associações simples

2. **Intermediário:**
   - Sistema de e-commerce com include e extend
   - Implementar herança de atores
   - Criar especificação textual completa

3. **Avançado:**
   - Sistema completo de gestão hospitalar
   - Múltiplos níveis de herança
   - Documentação completa de requisitos

---

## 📌 **Dicas Importantes**

### ✅ **Boas Práticas:**
- Casos de uso devem ser verbos (Cadastrar, Consultar, Alterar)
- Atores são substantivos (Cliente, Gerente, Sistema)
- Mantenha diagramas simples e claros
- Use include para evitar repetição
- Use extend para funcionalidades opcionais

### ❌ **Erros Comuns:**
- Confundir atributos com casos de uso
- Criar associação entre atores
- Criar associação entre casos de uso (use include/extend)
- Diagramas muito complexos e difíceis de ler
- Não documentar as regras de negócio

---

## 🚀 **Próximos Passos**

- [ ] Adicionar diagramas completos
- [ ] Criar exercícios resolvidos
- [ ] Adicionar templates de documentação
- [ ] Criar projeto final completo
- [ ] Tutorial de StarUML

---

## 📚 **Relação com Outras Disciplinas**

- **POO:** Casos de uso se tornam classes
- **Banco de Dados:** Atributos viram tabelas
- **Desenvolvimento:** Casos de uso viram funcionalidades do código

---

<div align="center">

**📗 Material do 3º Período - TSI**

[⬅️ Voltar ao índice principal](../../README.md)

</div>
