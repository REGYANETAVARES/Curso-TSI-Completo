# 📘 Algoritmos e Programação

> **1º Período - Professor Pereira**  
> Fundamentos de programação, estruturas de repetição, funções e recursividade

---

## 📋 **Sobre a Disciplina**

Disciplina introdutória de programação que aborda os conceitos fundamentais de algoritmos, estruturas de controle, modularização de código através de funções e procedimentos, e técnicas avançadas como recursividade.

---

## 🎯 **Objetivos de Aprendizado**

- Compreender estruturas de repetição (while, do-while, for)
- Dominar a criação e uso de funções e procedimentos
- Entender a diferença entre funções (return) e procedimentos (void)
- Aplicar recursividade em problemas práticos
- Desenvolver lógica de programação
- Otimizar código através de modularização

---

## 📚 **Conteúdo Programático**

### **Módulo 1: Estruturas de Repetição**
- While no início vs While no final
- Laço for
- Comparação entre estruturas

### **Módulo 2: Funções e Procedimentos**
- Conceito de modularização
- Procedimentos (void)
- Funções com retorno
- Argumentos e parâmetros
- Escopo de variáveis

### **Módulo 3: Aplicações Práticas**
- Sistema de cálculo de FGTS
- Folha de pagamento
- Descontos e cálculos financeiros
- Trabalho com vetores

### **Módulo 4: Recursividade**
- Conceito de função recursiva
- Substituição de loops por recursão
- Exemplos práticos
- Quando usar recursividade

---

## 📂 **Estrutura de Arquivos**

```
Algoritmos-Programacao/
├── README.md (este arquivo)
├── aulas-transcritas/
│   ├── pereira.pdf          # Orientações gerais
│   ├── pereira_1.pdf         # Estruturas de repetição
│   ├── pereira_2.pdf         # Funções e FGTS
│   ├── pereira_3.pdf         # Continuação funções
│   ├── pereira_4.pdf         # Funções com vetores
│   └── pereira_5.pdf         # Recursividade
├── exercicios/
│   └── (exercícios a serem adicionados)
└── codigos/
    └── (códigos-fonte a serem adicionados)
```

---

## 🎓 **Aulas Disponíveis**

### **Aula 1: Orientações Gerais**
- Informações sobre avaliação
- Metodologia da disciplina

### **Aula 2: Estruturas de Repetição**
- Diferença entre while no início e while no final
- Como escolher a estrutura adequada
- Exemplos práticos

### **Aula 3: Introdução a Funções**
- Divisão de programas em blocos
- Conceito de procedimentos (void)
- Conceito de funções (com retorno)
- Gerenciamento de memória

### **Aula 4: Sistema de FGTS**
- Cálculo prático de FGTS
- Funções com argumentos
- Retorno de valores
- Exemplo completo de folha de pagamento

### **Aula 5: Funções com Vetores**
- Passagem de vetores para funções
- Sistema de cadastro de funcionários
- Cálculo de FGTS e adiantamentos
- Salário líquido

### **Aula 6: Recursividade**
- Conceito de função recursiva
- Substituição de estruturas de repetição
- Exemplos: sequência numérica, soma de pares
- Quando usar recursividade vs loops

---

## 💡 **Conceitos-Chave**

### **Procedimentos vs Funções**

| Característica | Procedimento (void) | Função |
|----------------|---------------------|--------|
| Retorna valor? | ❌ Não | ✅ Sim |
| Sintaxe | `void nomeProcedimento()` | `tipo nomeFuncao()` |
| Uso | Executar ações | Calcular e retornar |
| Comando | - | `return valor;` |

### **Exemplo Prático: FGTS**

```c
// Função que calcula FGTS
float calcularFGTS(float salario) {
    float fgts;
    fgts = salario * 0.08; // 8% do salário
    return fgts;
}

// Uso da função
int main() {
    float salario, valorFGTS;
    printf("Digite o salário: ");
    scanf("%f", &salario);
    
    valorFGTS = calcularFGTS(salario);
    printf("FGTS: R$ %.2f\n", valorFGTS);
    
    return 0;
}
```

---

## 🎯 **Aplicações Práticas**

### **Sistema de Folha de Pagamento**
- Cálculo de FGTS (8% do salário bruto)
- Cálculo de INSS (conforme tabela)
- Cálculo de Imposto de Renda
- Adiantamentos salariais
- Salário líquido final

### **Vantagens da Modularização**
- ✅ Código mais organizado
- ✅ Reutilização de funções
- ✅ Facilita manutenção
- ✅ Melhor gerenciamento de memória
- ✅ Código mais legível

---

## 📖 **Recursos Adicionais**

### **Linguagens Abordadas**
- C (linguagem principal)
- Conceitos aplicáveis a outras linguagens

### **Comparação com Outras Linguagens**
- PHP: Não precisa declarar tipos, funções automáticas
- Java: Orientação a objetos, conceitos similares
- Python: Sintaxe mais simples, mesmos conceitos

---

## ✍️ **Exercícios Recomendados**

1. **Básico:**
   - Criar função para calcular área de triângulo
   - Criar função para calcular desconto
   - Imprimir sequência de números com recursividade

2. **Intermediário:**
   - Sistema completo de cálculo de FGTS
   - Função para calcular salário líquido
   - Cadastro de múltiplos funcionários com vetores

3. **Avançado:**
   - Sistema completo de folha de pagamento
   - Implementar recursividade para substituir todos os loops
   - Criar biblioteca de funções reutilizáveis

---

## 🚀 **Próximos Passos**

- [ ] Adicionar códigos-fonte completos
- [ ] Criar exercícios resolvidos
- [ ] Adicionar exemplos práticos
- [ ] Criar projeto final integrador
- [ ] Adicionar videoaulas complementares

---

## 👨‍🏫 **Sobre o Professor**

**Professor Pereira**
- Ensino didático e prático
- Foco em aplicações reais (FGTS, folha de pagamento)
- Ênfase em boas práticas de programação

---

## 📌 **Observações Importantes**

1. **Funções não deixam "lixo" na memória** - quando a função termina, suas variáveis locais são automaticamente liberadas
2. **Procedimentos vs Funções**: Use procedimentos quando só precisa executar ações; use funções quando precisa retornar um valor
3. **Recursividade**: Poderosa mas deve ser usada com cuidado - nem sempre é mais eficiente que loops
4. **Variáveis globais**: Evite! Podem causar problemas difíceis de debugar

---

<div align="center">

**📚 Material do 1º Período - TSI**

[⬅️ Voltar ao índice principal](../../README.md)

</div>
