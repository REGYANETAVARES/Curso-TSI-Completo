# 📙 Programação Orientada a Objetos (POO)

> **3º Período - Professores Marcel e Leila**  
> Conceitos fundamentais de POO: classes, objetos, estado, construtores, agregação e composição

---

## 📋 **Sobre a Disciplina**

Disciplina que aborda os fundamentos da Programação Orientada a Objetos, incluindo conceitos de classes, objetos, estado de objetos, construtores, agregação, composição e generalização. Material ministrado por dois professores com abordagens complementares.

---

## 🎯 **Objetivos de Aprendizado**

- Compreender o conceito de classes e objetos
- Entender estado de objetos e como ele muda
- Dominar construtores e instanciação
- Aplicar agregação e composição
- Diferenciar modelo estático de modelo dinâmico
- Implementar conceitos de POO em Java

---

## 📚 **Conteúdo Programático**

### **Módulo 1: Estado de Objetos (Professor Marcel)**
- Conceito de estado atual
- Analogia da "foto da memória"
- Mudanças de estado
- Exemplos práticos (iFood, aluno)

### **Módulo 2: Classes e Objetos (Professora Leila)**
- Diferença entre classe e objeto
- Construtores
- Atributos e métodos
- Instanciação

### **Módulo 3: Relacionamentos (Professora Leila)**
- Agregação
- Composição
- Generalização
- Modelo estático vs dinâmico

---

## 📂 **Estrutura de Arquivos**

```
POO/
├── README.md (este arquivo)
├── aulas-transcritas/
│   ├── 01-marcel-estado-objetos.pdf/.docx
│   ├── 02-marcel-estados-ifood.pdf/.docx
│   ├── 03-marcel-variaveis-estados.pdf/.docx
│   ├── 04-leila-classes-objetos.docx
│   └── 05-leila-agregacao-composicao.docx
├── exercicios/
│   └── (exercícios a serem adicionados)
└── projetos/
    └── (projetos a serem adicionados)
```

---

## 🎓 **Aulas Disponíveis**

### **👨‍🏫 Professor Marcel - Estado de Objetos**

#### **Aula 1: Conceito de Estado**
- O que é um objeto (material vs abstrato)
- Características, comportamentos e estado
- Analogia da "foto da memória"
- Estado atual como snapshot do objeto

**Conceitos principais:**
- Estado é o valor das variáveis do objeto em um momento específico
- Estado pode mudar ao longo do tempo
- Cada objeto tem seu próprio estado

#### **Aula 2: Estados Múltiplos - Exemplo iFood**
- Estados de um pedido
- Transições entre estados
- Exemplo prático de sistema real

**Estados de um Pedido:**
1. Criado
2. Pendente (aguardando aprovação)
3. Aprovado
4. Em preparação
5. Saiu para entrega
6. Entregue

#### **Aula 3: Variáveis e Estados**
- Objetos podem ter estados diferentes
- Objetos podem ter estados iguais
- Duas variáveis podem apontar para o mesmo objeto

---

### **👩‍🏫 Professora Leila - Classes, Objetos e Relacionamentos**

#### **Aula 4: Classes e Objetos**
- Definição de classe
- Definição de objeto
- Construtores
- Instanciação
- Exemplo: Classe Carro

**Estrutura:**
```java
class Carro {
    // Atributos
    private String modelo;
    private String cor;
    private int ano;
    
    // Construtor
    public Carro(String modelo, String cor, int ano) {
        this.modelo = modelo;
        this.cor = cor;
        this.ano = ano;
    }
    
    // Métodos
    public void acelerar() { ... }
    public void frear() { ... }
}

// Criando objeto (instanciando)
Carro carro1 = new Carro("Civic", "Preto", 2023);
```

#### **Aula 5: Agregação, Composição e Generalização**
- Diferença entre agregação e composição
- Quando usar cada uma
- Modelo estático vs modelo dinâmico
- Importância da estrutura do sistema

**Conceitos:**
- **Agregação:** Relação "tem-um" (pode existir independentemente)
- **Composição:** Relação "parte-de" (não existe sem o todo)
- **Generalização:** Herança, hierarquia de classes

---

## 💡 **Conceitos-Chave**

### **Classe vs Objeto**

| Aspecto | Classe | Objeto |
|---------|--------|--------|
| O que é | Modelo/Template | Instância concreta |
| Exemplo | "Carro" | "Meu Civic preto 2023" |
| Na memória | Não ocupa espaço | Ocupa espaço |
| Quantidade | Uma definição | Múltiplas instâncias |

### **Estado de um Objeto**

```
ANALOGIA: FOTO DA MEMÓRIA

Imagine que você pode tirar uma "foto" da memória 
no momento exato em que o objeto existe.

Exemplo: Aluno
- Nome: "João Silva"
- Endereço: "Rua A, 123"
- Matrícula: "2024001"

Se o aluno mudar de endereço:
- ANTES: Estado 1 (Rua A, 123)
- DEPOIS: Estado 2 (Rua B, 456)

O objeto é o mesmo, mas o ESTADO mudou!
```

### **Construtor**

O construtor é o método especial que **constrói** (cria) o objeto na memória.

```java
// Construtor
public Aluno(String nome, String endereco) {
    this.nome = nome;
    this.endereco = endereco;
}

// Criando objeto (chamando o construtor)
Aluno aluno1 = new Aluno("João", "Rua A, 123");
```

---

## 🎯 **Exemplos Práticos**

### **Exemplo 1: Sistema de Pedidos (iFood)**

```java
class Pedido {
    private int numero;
    private String status;
    private List<Item> itens;
    
    // Estados possíveis:
    // "CRIADO", "PENDENTE", "APROVADO", 
    // "PREPARANDO", "ENTREGANDO", "ENTREGUE"
    
    public void aprovar() {
        this.status = "APROVADO";
    }
    
    public void prepararPedido() {
        this.status = "PREPARANDO";
    }
    
    public String getStatus() {
        return this.status;
    }
}
```

### **Exemplo 2: Sistema de Alunos**

```java
class Aluno {
    private String nome;
    private String matricula;
    private String endereco;
    
    // Construtor
    public Aluno(String nome, String matricula, String endereco) {
        this.nome = nome;
        this.matricula = matricula;
        this.endereco = endereco;
    }
    
    // Método que muda o estado
    public void mudarEndereco(String novoEndereco) {
        this.endereco = novoEndereco;
        // ESTADO DO OBJETO MUDOU!
    }
}

// Uso:
Aluno aluno = new Aluno("Maria", "2024001", "Rua A");
System.out.println(aluno.getEndereco()); // "Rua A" (Estado 1)

aluno.mudarEndereco("Rua B");
System.out.println(aluno.getEndereco()); // "Rua B" (Estado 2)
```

---

## 📖 **Agregação vs Composição**

### **Agregação** (Relação "tem-um")
O objeto pode existir independentemente.

```java
class Departamento {
    private List<Professor> professores; // Agregação
}
// Professor pode existir sem Departamento
```

### **Composição** (Relação "parte-de")
O objeto não existe sem o todo.

```java
class Casa {
    private List<Comodo> comodos; // Composição
}
// Se Casa é destruída, Cômodos também são
```

---

## 📊 **Modelo Estático vs Modelo Dinâmico**

### **Modelo Estático (Estrutural)**
- Define a estrutura das classes
- Atributos e métodos
- Relacionamentos entre classes
- **Difícil de mudar depois de implementado**

```java
class Cliente {
    private String nome;
    private String cpf;
    // Estrutura básica
}
```

### **Modelo Dinâmico (Comportamental)**
- Define como objetos interagem
- Fluxos de execução
- Mudanças de estado
- **Mais fácil de ajustar**

```java
// Interação entre objetos
cliente.fazerPedido();
pedido.processar();
pagamento.confirmar();
```

---

## 🔍 **Pilares de POO (Preview)**

Embora não sejam o foco principal destas aulas, os 4 pilares de POO são:

1. **Encapsulamento** - Esconder detalhes internos
2. **Herança** - Reutilizar código através de hierarquias
3. **Polimorfismo** - Múltiplas formas de um mesmo método
4. **Abstração** - Simplificar complexidade

---

## ✍️ **Exercícios Recomendados**

### **Básico:**
1. Criar classe `Carro` com atributos e construtor
2. Instanciar 3 objetos diferentes
3. Demonstrar mudança de estado

### **Intermediário:**
1. Criar classe `ContaBancaria` com saldo
2. Implementar métodos `depositar()` e `sacar()`
3. Demonstrar mudanças de estado do saldo

### **Avançado:**
1. Sistema de biblioteca completo
2. Classes: Livro, Usuario, Emprestimo
3. Demonstrar agregação e composição
4. Implementar mudanças de estado

---

## 🚀 **Próximos Passos na Disciplina**

- [ ] Herança e polimorfismo
- [ ] Interfaces e classes abstratas
- [ ] Exceções e tratamento de erros
- [ ] Collections (List, Set, Map)
- [ ] Projeto prático integrador

---

## 🎓 **Professores**

### **Professor Marcel**
- Foco em conceitos fundamentais
- Exemplos do dia a dia (iFood)
- Didática clara com analogias

### **Professora Leila**
- Abordagem técnica e estrutural
- Ênfase em boas práticas
- Preparação para projetos reais

---

## 📌 **Observações Importantes**

1. **Estado é dinâmico** - pode mudar a qualquer momento
2. **Classe é estática** - define a estrutura
3. **Objeto é concreto** - existe na memória
4. **Construtor sempre tem o mesmo nome da classe**
5. **Modelo estático deve ser bem planejado** - base do sistema

---

## 💡 **Dicas de Estudo**

- ✅ Pratique criando classes do zero
- ✅ Desenhe diagramas de classe (UML)
- ✅ Pense em objetos do mundo real
- ✅ Teste mudanças de estado
- ✅ Compare com Modelagem de Sistemas (UML)

---

## 📚 **Relação com Outras Disciplinas**

- **UML:** Casos de uso viram classes
- **Banco de Dados:** Atributos viram colunas
- **Estrutura de Dados:** Collections usam POO

---

<div align="center">

**📙 Material do 3º Período - TSI**

[⬅️ Voltar ao índice principal](../../README.md)

</div>
