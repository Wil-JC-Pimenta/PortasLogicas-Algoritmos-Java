# Estudo sobre Portas Lógicas

## Aplicações em Circuitos Digitais e Lógica de Programação

---

### Sumário

1. Introdução  
   1.1 A Importância das Portas Lógicas  
   1.2 Operadores Lógicos em Diversas Linguagens de Programação  
   1.3 Conceitos de Sinal Binário (0 e 1)  
   1.4 Relevância da Lógica Booleana  
   1.5 Inter-relação entre Circuitos Digitais e Fluxos de Decisão em Algoritmos
2. Descrição Detalhada de Cada Porta Lógica
   2.1 Porta AND (E)
   2.2 Porta OR (OU)
   2.3 Porta NOT (NÃO)
   2.4 Porta NAND (NÃO-E)
   2.5 Porta NOR (NÃO-OU)
   2.6 Porta XOR (OU Exclusivo)
   2.7 Porta XNOR (NÃO-OU Exclusivo)
3. Aplicação em Lógica de Programação com Java
   3.1 Operadores Booleanos em Java
   3.2 Exemplos com Estruturas Condicionais (if/else)
   3.3 Declaração de Variáveis Booleanas e Operações Diretas
   3.4 Estruturas switch-case para Operações Lógicas
4. Relação entre Circuitos Digitais e Algoritmos
   4.1 Analogia entre Circuitos e Algoritmos
   4.2 Representação de Circuitos como Algoritmos
   4.3 Fluxogramas: Do Circuito ao Algoritmo
   4.4 Casos Práticos
5. Conclusão

---

## 1. Introdução

### 1.1 A Importância das Portas Lógicas

As portas lógicas são os blocos fundamentais da eletrônica digital moderna e, por extensão, dos computadores e dispositivos eletrônicos que permeiam nossa sociedade. Estes componentes formam a base de todos os circuitos digitais, desde simples calculadoras até supercomputadores complexos.

No âmbito da eletrônica digital, as portas lógicas são circuitos eletrônicos que implementam operações booleanas básicas. Elas são os componentes essenciais que permitem a construção de sistemas mais complexos como registradores, contadores, multiplexadores, somadores e, eventualmente, microprocessadores completos.

![Portas Lógicas](/markdown/img/portas-logicas.png)

Na programação, as portas lógicas se manifestam como operadores que, por meio de expressões booleanas avaliando "verdadeiro" ou "falso", controlam o fluxo de execução dos algoritmos. Ao combiná-las (utilizando AND, OR, NOT, entre outros), os programadores criam estruturas condicionais, como if/else, loops e switch/case, que permitem tomar decisões com base em múltiplos critérios.<br>
Essa abordagem, fundamentada na álgebra booleana e em técnicas de simplificação como as leis de De Morgan, não só torna o código mais eficiente e organizado, como também é essencial em aplicações que vão desde o desenvolvimento de software até a implementação de sistemas embarcados e controle de hardware.

![Tabela Verdade - Operadores Lógicos](/markdown/img/tabela-verdade-operadores-logicos.jpg)

### 1.2 Operadores Lógicos em Diversas Linguagens de Programação

---

## ✅ C e C++

(Em C e C++ os operadores são idênticos.)

<table>
  <thead>
    <tr>
      <th>Operador</th>
      <th>Significado</th>
      <th>Exemplo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>&&</code></td>
      <td>E lógico (AND)</td>
      <td><code>a && b</code></td>
    </tr>
    <tr>
      <td><code>||</code></td>
      <td>OU lógico (OR)</td>
      <td><code>a || b</code></td>
    </tr>
    <tr>
      <td><code>!</code></td>
      <td>NÃO lógico (NOT)</td>
      <td><code>!a</code></td>
    </tr>
  </tbody>
</table>

---

## ✅ Java

(Os operadores são os mesmos de C/C++.)

<table>
  <thead>
    <tr>
      <th>Operador</th>
      <th>Significado</th>
      <th>Exemplo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>&&</code></td>
      <td>E lógico (AND)</td>
      <td><code>a && b</code></td>
    </tr>
    <tr>
      <td><code>||</code></td>
      <td>OU lógico (OR)</td>
      <td><code>a || b</code></td>
    </tr>
    <tr>
      <td><code>!</code></td>
      <td>NÃO lógico (NOT)</td>
      <td><code>!a</code></td>
    </tr>
  </tbody>
</table>

> **Obs:** Java também possui <code>&</code> e <code>|</code> para operações bit a bit, mas <code>&&</code> e <code>||</code> são usados para lógica booleana.

---

## ✅ JavaScript

<table>
  <thead>
    <tr>
      <th>Operador</th>
      <th>Significado</th>
      <th>Exemplo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>&&</code></td>
      <td>E lógico (AND)</td>
      <td><code>a && b</code></td>
    </tr>
    <tr>
      <td><code>||</code></td>
      <td>OU lógico (OR)</td>
      <td><code>a || b</code></td>
    </tr>
    <tr>
      <td><code>!</code></td>
      <td>NÃO lógico (NOT)</td>
      <td><code>!a</code></td>
    </tr>
  </tbody>
</table>

> **Obs:** <code>&&</code> e <code>||</code> podem retornar o próprio valor (curto-circuito), não apenas <code>true</code> ou <code>false</code>.

---

## ✅ Python

```plaintext
| Operador |   Significado    |  Exemplo  |
| :------: | :--------------: | :-------: |
|  `and`   |  E lógico (AND)  | `a and b` |
|   `or`   |  OU lógico (OR)  | `a or b`  |
|  `not`   | NÃO lógico (NOT) |  `not a`  |
```

### 1.3 Conceitos de Sinal Binário (0 e 1)

O sistema digital baseia-se fundamentalmente no conceito binário, onde todas as informações são representadas por apenas dois estados: 0 e 1 (também referidos como "baixo" e "alto", "falso" e "verdadeiro", ou "desligado" e "ligado").

Esta simplicidade é o que torna os sistemas digitais tão robustos e confiáveis.

Em termos de hardware, estes valores binários são tipicamente representados por níveis de tensão:

```plaintext
• O valor lógico 0 (baixo) geralmente corresponde a 0V ou tensão próxima de zero.

• O valor lógico 1 (alto) geralmente corresponde a uma tensão positiva (como 3.3V, 5V ou outros valores, dependendo da tecnologia).
```

Em termos de software, estes valores são representados por tipos de dados booleanos, onde:

```plaintext
• false corresponde a 0

• true corresponde a 1
```

### 1.4 Relevância da Lógica Booleana

A lógica booleana, desenvolvida pelo matemático George Boole no século XIX, fornece o modelo matemático que fundamenta toda a eletrônica digital e a ciência da computação.
Esta álgebra trabalha com valores binários (verdadeiro ou falso) e define um conjunto de operações que podem ser realizadas com estes valores.

As três operações fundamentais da álgebra booleana são:

```plaintext
• AND (E): Resulta em verdadeiro apenas se ambos os operandos forem verdadeiros.

• OR (OU): Resulta em verdadeiro se pelo menos um dos operandos for verdadeiro.

• NOT (NÃO): Inverte o valor lógico (verdadeiro torna-se falso e vice-versa).
```

A partir destas operações básicas, podem ser derivadas outras operações como NAND, NOR, XOR e XNOR.

### 1.5 Inter-relação entre Circuitos Digitais e Fluxos de Decisão em Algoritmos

Existe uma relação intrínseca entre circuitos digitais e algoritmos. Ambos processam informações e tomam decisões baseadas em lógica booleana:

```plaintext
• Um circuito digital recebe sinais de entrada, processa-os através de portas lógicas e produz sinais de saída.

• Um algoritmo recebe dados de entrada, processa-os através de operações lógicas e aritméticas, e produz resultados de saída.
```

Esta analogia não é coincidência. Os computadores digitais foram projetados para executar algoritmos, e suas estruturas internas de hardware refletem diretamente as estruturas lógicas dos algoritmos que executam.

Por exemplo, quando um programador escreve uma declaração condicional como if (A && B), o hardware do computador utiliza portas AND físicas (ou seus equivalentes em transistores) para avaliar esta condição.

## 2. Descrição Detalhada de Cada Porta Lógica

### 2.1 Porta AND (E)

#### Definição e Funcionamento

A porta AND produz uma saída de valor 1 (verdadeiro) apenas quando todas as suas entradas são 1 (verdadeiras). Em qualquer outro caso, a saída é 0 (falso).

#### Símbolo Gráfico

```plaintext
A ---+
     |D--- Y = A AND B
B ---+
```

![Porta Lógica AND](/markdown/img/porta-logica-and-1.png)

O símbolo da porta AND assemelha-se a um D com a parte plana à direita, tendo duas ou mais entradas à esquerda e uma saída à direita.

#### Expressão Algébrica

```plaintext
Y = A · B (ou A AND B)
```

Em Java:

```java
Y = A && B
```

##### Tabela Verdade (para 2 entradas)

```plaintext
A B Y (Saída)
0 0 0
0 1 0
1 0 0
1 1 1
```

#### Exemplo de Circuito Básico

Um exemplo típico de aplicação da porta AND é um circuito de segurança onde dois sensores (A e B) devem estar ativos simultaneamente para permitir o acesso. Somente quando ambos os sensores detectam uma condição (como um cartão de acesso válido E uma impressão digital correta), o sistema permite a entrada.

### 2.2 Porta OR (OU)

#### Definição e Funcionamento

A porta OR produz uma saída de valor 1 (verdadeiro) quando pelo menos uma de suas entradas é 1 (verdadeira).
A saída é 0 (falso) apenas quando todas as entradas são 0 (falsas).

#### Símbolo Gráfico

```plaintext
    A ---\
         |>--- Y = A OR B<br>
    B ---/
```

O símbolo da porta OR assemelha-se a uma seta apontando para a direita com uma curvatura convexa na entrada.

![Porta Lógica OR(OU)](/markdown/img/porta-or-1.png)

### Expressão Algébrica

```plaintext
Y = A + B (ou A OR B)
```

Em Java:

```java
Y = A || B
```

#### Tabela Verdade (para 2 entradas)

```plaintext
A B Y (Saída)
0 0 0
0 1 1
1 0 1
1 1 1
```

### Exemplo de Circuito Básico

Um exemplo prático de porta OR é um sistema de alarme de incêndio onde múltiplos sensores (A, B, C, etc.) monitoram diferentes áreas. Se qualquer um dos sensores detectar fumaça ou calor, o alarme dispara.

## 2.3 Porta NOT (NÃO)

### Definição e Funcionamento

A porta NOT, também chamada de inversor, tem apenas uma entrada e uma saída. Ela inverte o valor lógico da entrada: se a entrada for 1, a saída será 0; se a entrada for 0, a saída será 1.

### Símbolo Gráfico

```plaintext
A ---o--- Y = NOT A
```

![Porta Lógica NOT](/markdown/img/porta-not.png)

### Expressão Algébrica

```plaintext
Y = Ā (ou NOT A)
```

Em Java:

```java
Y = !A
```

#### Tabela Verdade

```plaintext
A Y(Saída)
0 1
1 0
```

### Exemplo de Circuito Básico

A porta NOT é frequentemente usada em sistemas de controle para inverter sinais. Por exemplo, em um sistema de alarme, quando uma porta está fechada, o sensor pode enviar um sinal 1; quando a porta está aberta, o sinal é 0.
Uma porta NOT pode ser usada para transformar este sinal em um indicador "porta aberta" (1 quando aberta).

## 2.4 Porta NAND (NÃO-E)

### Definição e Funcionamento

A porta NAND é a negação da porta AND. Ela produz uma saída 0 (falso) apenas quando todas as suas entradas são 1 (verdadeiras). Em todos os outros casos, a saída é 1 (verdadeiro).

#### Símbolo Gráfico

```plaintext
A ---+
|    |D--o--- Y = A NAND B
B ---+
```

![Porta Lógica NAND(NÃO-E)](/markdown/img/porta-logica-nand.png)

O símbolo da porta NAND é idêntico ao da porta AND, mas com um pequeno círculo na saída.

### Expressão Algébrica

```plaintext
Y = (A · B)̄ (ou A NAND B)
```

Em Java:

```java
Y = !(A && B)
```

## Tabela Verdade (para 2 entradas)

```plaintext
A B Y(Saída)
0 0 1
0 1 1
1 0 1
1 1 0
```

## Exemplo de Circuito Básico

A porta NAND é considerada uma porta universal, pois qualquer função lógica pode ser implementada usando apenas portas NAND. Um exemplo prático é um circuito de trava eletrônica que ativa um alarme quando ambas as portas de segurança estão abertas simultaneamente.

## 2.5 Porta NOR (NÃO-OU)

### Definição e Funcionamento

A porta NOR é a negação da porta OR. Ela produz uma saída 1 (verdadeiro) apenas quando todas as suas entradas são 0 (falsas). Em todos os outros casos, a saída é 0 (falso).

#### Símbolo Gráfico

#### Símbolo Gráfico

```plaintext
A ---\
|>--o--- Y = A NOR B
B ---/
```

![Porta Lógica NOR(NÃO-OU)](/markdown/img/porta-logica-nor.png)

O símbolo da porta NOR é idêntico ao da porta OR, mas com um pequeno círculo na saída.

### Expressão Algébrica

```plaintext
Y = (A + B)̄ (ou A NOR B)
```

Em Java:

```java
Y = !(A || B)
```

#### Tabela Verdade (para 2 entradas)

```plaintext
A B Y(Saída)
0 0 1
0 1 0
1 0 0
1 1 0
```

### Exemplo de Circuito Básico

Assim como a porta NAND, a porta NOR também é uma porta universal. Um exemplo de aplicação é um sistema de economia de energia que desliga automaticamente um equipamento quando nenhum de seus sensores de movimento detecta atividade por um determinado período.

## 2.6 Porta XOR (OU Exclusivo)

### Definição e Funcionamento

A porta XOR (Exclusive OR) produz uma saída 1 (verdadeiro) quando exatamente uma de suas entradas é 1 (verdadeira). Se ambas as entradas forem iguais (ambas 0 ou ambas 1), a saída é 0 (falso).

### Símbolo Gráfico

```plaintext
A ---\
|>--- Y = A XOR B
B ---/
```

![Porta Lógica XOR(OU EXCLUSIVO)](/markdown/img/porta-logica-xor.png)

O símbolo da porta XOR é semelhante ao da porta OR, mas com uma linha adicional paralela à entrada curva.

### Expressão Algébrica

````plaintext
Y = A ⊕ B (ou A XOR B)
```plaintext

Em Java:

```java
Y = A ^ B
````

#### Tabela Verdade (para 2 entradas)

```plaintext
A B Y(Saída)
0 0 0
0 1 1
1 0 1
1 1 0
```

### Exemplo de Circuito Básico

A porta XOR é frequentemente usada em circuitos aritméticos, como em um somador de bits onde a saída do XOR representa a soma sem considerar o carry. Outro exemplo é um circuito de detecção de paridade, usado para verificar erros em transmissão de dados.

## 2.7 Porta XNOR (NÃO-OU Exclusivo)

### Definição e Funcionamento

A porta XNOR é a negação da porta XOR. Ela produz uma saída 1 (verdadeiro) quando ambas as entradas são iguais (ambas 0 ou ambas 1). Se as entradas forem diferentes, a saída é 0 (falso).

### Símbolo Gráfico

```plaintext
A ---\
|>--o--- Y = A XNOR B
B ---/
```

![Porta Lógica XNOR(OU EXCLUSIVO NÃO)](/markdown/img/porta-logica-xor.png)

O símbolo da porta XNOR é idêntico ao da porta XOR, mas com um pequeno círculo na saída.

### Expressão Algébrica

```plaintext
Y = (A ⊕ B)̄ (ou A XNOR B)
```

Em Java:

```java
Y = !(A ^ B) ou Y = A == B
```

#### Tabela Verdade (para 2 entradas)

```plaintext
A B Y(Saída)
0 0 1
0 1 0
1 0 0
1 1 1
```

### Exemplo de Circuito Básico

A porta XNOR é útil em circuitos de comparação que verificam se dois sinais são idênticos.
Também é utilizada em circuitos de detecção de paridade par, onde a saída deve ser 1 quando o número total de 1's na entrada (incluindo o bit de paridade) é par.

## 3. Aplicação em Lógica de Programação com Java

### 3.1 Operadores Booleanos em Java

Em Java, os operadores lógicos permitem combinar expressões booleanas para criar condições mais complexas. Estes operadores têm uma correspondência direta com as portas lógicas estudadas na eletrônica digital.

**Porta Lógica:** AND  
**Operador em Java:** `&&`  
**Significado:** E Lógico

**Porta Lógica:** OR  
**Operador em Java:** `||`  
**Significado:** OU Lógico

**Porta Lógica:** XNOR  
**Operador em Java:** `==` (booleanos)  
**Significado:** OU Exclusivo NÃO (simulado)

**Porta Lógica:** XOR  
**Operador em Java:** `^`  
**Significado:** OU Exclusivo (bit a bit)

**Observações:**

As portas NAND, NOR e XNOR não têm operadores dedicados em Java, mas podem ser implementadas combinando os operadores básicos.

```plaintext
- O operador `^` (XOR) em Java realiza a operação de OU Exclusivo **bit a bit**. Para aplicar XOR a booleanos, utiliza-se a expressão lógica `(a || b) && !(a && b)`.

- Não existe um operador nativo para XNOR em Java. No entanto, para valores booleanos, o operador `==` pode ser utilizado para simular a operação de OU Exclusivo NÃO, pois retorna `true` quando ambos os valores são iguais (`true == true` ou `false == false`).
```

## 3.2 Exemplos com Estruturas Condicionais (if/else)

### Porta AND em Java

```java
  // Exemplo de AND lógico em controle de acesso
  public boolean verificarAcesso(boolean temCartao, boolean digitouSenhaCorreta) {
  // Acesso concedido apenas se tiver cartão E a senha estiver correta
  if (temCartao && digitouSenhaCorreta) {
  System.out.println("Acesso concedido!");
  return true;
  } else {
  System.out.println("Acesso negado!");
  return false;
  }
  }

```

### Porta OR em Java

```java
  // Exemplo de OR lógico em sistema de notificação
public void notificarUsuario(boolean temNovoEmail, boolean temNovaMensagem) {
    // Notifica se houver novo email OU nova mensagem
    if (temNovoEmail || temNovaMensagem) {
        System.out.println("Você tem novas notificações!");
    } else {
        System.out.println("Nenhuma notificação nova.");
    }
}
```

### Porta NOT em Java

```java
// Exemplo de NOT lógico em controle de estado
public void controlarEstado(boolean sistemaLigado) {
    // Inverte o estado atual
    boolean novoEstado = !sistemaLigado;
    System.out.println("Estado anterior: " + (sistemaLigado ? "Ligado" : "Desligado"));
    System.out.println("Novo estado: " + (novoEstado ? "Ligado" : "Desligado"));
}
```

### Combinação de Portas Lógicas em Java

```java
// Exemplo de NAND lógico (combinação de AND e NOT)
public boolean verificarAlarme(boolean sensor1Ativado, boolean sensor2Ativado) {
    // O alarme dispara se não for verdade que ambos os sensores estão ativados
    // Implementação de NAND: !(sensor1Ativado && sensor2Ativado)
    boolean resultado = !(sensor1Ativado && sensor2Ativado);
    if (resultado) {
        System.out.println("Alarme disparado!");
        return true;
    } else {
        System.out.println("Sistema seguro.");
        return false;
    }
}
```

# 3.3 Declaração de Variáveis Booleanas e Operações Diretas

```java
public class OperacoesLogicas {
    public static void main(String[] args) {
        // Declaração de variáveis booleanas
        boolean a = true;
        boolean b = false;

        // Operações lógicas básicas
        boolean resultadoAND = a && b;
        boolean resultadoOR = a || b;
        boolean resultadoNOT_A = !a;
        boolean resultadoXOR = a ^ b;

        // Operações lógicas derivadas
        boolean resultadoNAND = !(a && b);
        boolean resultadoNOR = !(a || b);
        boolean resultadoXNOR = !(a ^ b);

        // Exibição dos resultados
        System.out.println("A = " + a);
        System.out.println("B = " + b);
        System.out.println("A AND B = " + resultadoAND);
        System.out.println("A OR B = " + resultadoOR);
        System.out.println("NOT A = " + resultadoNOT_A);
        System.out.println("A XOR B = " + resultadoXOR);
        System.out.println("A NAND B = " + resultadoNAND);
        System.out.println("A NOR B = " + resultadoNOR);
        System.out.println("A XNOR B = " + resultadoXNOR);
    }
}
```

# 3.4 Estruturas switch-case para Operações Lógicas

```java
import java.util.Scanner;

public class CalculadoraLogica {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Calculadora de Operações Lógicas");
        System.out.println("--------------------------------");

        // Entrada de valores booleanos
        System.out.print("Digite o valor de A (true/false): ");
        boolean a = scanner.nextBoolean();
        System.out.print("Digite o valor de B (true/false): ");
        boolean b = scanner.nextBoolean();

        // Menu de operações
        System.out.println("\nEscolha a operação:");
        System.out.println("1. AND");
        System.out.println("2. OR");
        System.out.println("3. NOT A");
        System.out.println("4. NOT B");
        System.out.println("5. NAND");
        System.out.println("6. NOR");
        System.out.println("7. XOR");
        System.out.println("8. XNOR");
        System.out.print("\nDigite o número da operação: ");
        int operacao = scanner.nextInt();

        boolean resultado;
        String operacaoNome;

        // Utilizando switch-case para selecionar a operação
        switch (operacao) {
            case 1: // AND
                resultado = a && b;
                operacaoNome = "AND";
                break;
            case 2: // OR
                resultado = a || b;
                operacaoNome = "OR";
                break;
            case 3: // NOT A
                resultado = !a;
                operacaoNome = "NOT A";
                break;
            case 4: // NOT B
                resultado = !b;
                operacaoNome = "NOT B";
                break;
            case 5: // NAND
                resultado = !(a && b);
                operacaoNome = "NAND";
                break;
            case 6: // NOR
                resultado = !(a || b);
                operacaoNome = "NOR";
                break;
            case 7: // XOR
                resultado = a ^ b;
                operacaoNome = "XOR";
                break;
            case 8: // XNOR
                resultado = !(a ^ b);
                operacaoNome = "XNOR";
                break;
            default:
                System.out.println("Operação inválida.");
                return;
        }

        // Exibição do resultado
        System.out.println("\nResultado da operação " + operacaoNome + ": " + resultado);

        scanner.close();
    }
}
```

## 4. Relação entre Circuitos Digitais e Algoritmos

### 4.1 Analogia entre Circuitos e Algoritmos

Circuitos digitais e algoritmos são duas manifestações diferentes do mesmo conceito fundamental: o processamento lógico de informações. Esta relação pode ser entendida nos seguintes aspectos:

#### Elementos Fundamentais

```plaintext
• Circuitos Digitais: Utilizam portas lógicas como blocos de construção básicos.

• Algoritmos: Utilizam instruções como blocos de construção básicos.
```

#### Fluxo de Informação

```plaintext
• Circuitos Digitais: Sinais elétricos fluem através de componentes físicos.

• Algoritmos: Dados fluem através de instruções executadas sequencialmente.
```

#### Transformação de Entrada em Saída

```plaintext
• Circuitos Digitais: Transformam sinais de entrada em sinais de saída através de operações lógicas implementadas em hardware.

• Algoritmos: Transformam dados de entrada em dados de saída através de operações lógicas implementadas em software.
```

### 4.2 Representação de Circuitos como Algoritmos

Um circuito digital pode ser representado como um algoritmo seguindo estas etapas:

```plaintext
1. Identificar as entradas do circuito (variáveis booleanas)

2. Mapear as conexões entre portas lógicas como expressões booleanas

3. Traduzir as expressões booleanas em instruções condicionais

4. Definir as saídas do algoritmo com base nas avaliações dessas expressões
```

### Exemplo: Circuito Somador de 1 Bit

# Somador de 1 Bit

Um somador de 1 bit possui três entradas (A, B e Cin) e duas saídas (Sum e Cout).

**Circuito:**

- `Sum = A XOR B XOR Cin`
- `Cout = (A AND B) OR ((A XOR B) AND Cin)`

**Algoritmo em Java:**

```java
public class Somador1Bit {
    public boolean[] somar(boolean a, boolean b, boolean cIn) {
        // Cálculo da soma (XOR de três entradas)
        boolean sum = a ^ b ^ cIn;
        // Cálculo do carry out
        boolean cOut = (a && b) || ((a ^ b) && cIn);
        // Retorno das duas saídas em um array
        return new boolean[] { sum, cOut };
    }

    public static void main(String[] args) {
        Somador1Bit somador = new Somador1Bit();

        // Teste com A=1, B=1, Cin=0
        boolean a = true;
        boolean b = true;
        boolean cIn = false;

        boolean[] resultado = somador.somar(a, b, cIn);

        System.out.println("Entradas: A=" + a + ", B=" + b + ", Cin=" + cIn);
        System.out.println("Saídas: Sum=" + resultado[0] + ", Cout=" + resultado[1]);
    }
}
```

## 4.3 Fluxogramas: Do Circuito ao Algoritmo

Para ilustrar a transição de um circuito digital para um algoritmo, podemos utilizar fluxogramas que representam o mesmo processo lógico:

#### Representação de um Circuito AND-OR

```plaintext
Entrada A ---+
              |AND1---+
Entrada B ---+        |
                       |OR--- Saída
Entrada C ---+        |
              |AND2---+
Entrada D ---+
```

#### Fluxograma do Algoritmo Equivalente

```plaintext
[ Início ] → [ Ler A, B, C, D ] → [ Calcular AND1 = A AND B ]
            → [ Calcular AND2 = C AND D ]
            → [ Calcular Saída = AND1 OR AND2 ]
            → [ Exibir Saída ] → [ Fim ]
```

### Algoritmo em Java

```java
// Algoritmo em Java
public boolean calcularCircuito(boolean a, boolean b, boolean c, boolean d) {
    boolean and1 = a && b;
    boolean and2 = c && d;
    boolean saida = and1 || and2;
    return saida;
}
```

## 4.4 Casos Práticos

Exemplo 1: Sistema de Controle de Acesso

Descrição do Sistema: Um sistema de controle de acesso que verifica múltiplos fatores:

```plaintext
• Cartão de acesso válido (A)

• Senha correta (B)

• Horário autorizado (C)

• Não estar em lista de bloqueio (D)
```

#### Circuito Digital:

```plaintext
A ---+
     |AND1---+
B ---+       |
             |AND3--- Acesso Concedido
C ---+       |
     |AND2---+
D*---+
```

(D é invertido\* antes de entrar no AND2)

### Algoritmo em Java:

```java
public boolean verificarAcesso(
    boolean cartaoValido,
    boolean senhaCorreta,
    boolean horarioAutorizado,
    boolean estaNaListaDeBloqueio
) {
    // O acesso é concedido se:
    // (cartão válido E senha correta) E (horário autorizado E NÃO está na lista de bloqueio)
    boolean verificacaoCredenciais = cartaoValido && senhaCorreta;
    boolean verificacaoSeguranca = horarioAutorizado && !estaNaListaDeBloqueio;
    boolean acessoConcedido = verificacaoCredenciais && verificacaoSeguranca;
    return acessoConcedido;
}
```

### Exemplo 2: Sistema de Alarme

Descrição do Sistema: Um sistema de alarme que monitora:

```plaintext
• Sensor de movimento (A)

• Sensor de porta (B)

• Sensor de janela (C)

• Sistema está armado (D)
```

#### Circuito Digital

```plaintext

A ---+
     |
B ---+--OR1--+
     |       |
C ---+-------|AND--- Alarme Disparado
     |
D -----------+
```

```java
// Algoritmo em Java
public boolean verificarAlarme(
    boolean sensorMovimento,
    boolean sensorPorta,
    boolean sensorJanela,
    boolean sistemaArmado
) {    // O alarme dispara se:
  // Qualquer sensor for ativado E o sistema estiver armado
    boolean sensorAtivado = sensorMovimento || sensorPorta || sensorJanela;
   boolean alarmeDisparado = sensorAtivado && sistemaArmado;
    return alarmeDisparado;
}
```

## 5. Conclusão

O estudo de portas lógicas, álgebra booleana, algoritmos e lógica de programação com Java proporciona uma base sólida para o desenvolvimento de sistemas computacionais eficientes e inteligentes.  
Compreender o funcionamento das portas lógicas e a manipulação de variáveis booleanas é essencial para criar algoritmos mais seguros, otimizados e assertivos.  
Além disso, a prática com Java permite aplicar esses conceitos de maneira prática e moderna, preparando o desenvolvedor para enfrentar os desafios do mercado de tecnologia.

Agradecemos por acompanhar este material! Esperamos que ele tenha contribuído positivamente para seu aprendizado e evolução na área de desenvolvimento de sistemas.

---

Este projeto está licenciado sob a [Licença MIT](https://opensource.org/licenses/MIT).

**Desenvolvido por:**  
Wilker Junio Coelho Pimenta  
Curso de Análise e Desenvolvimento de Sistemas  
Universidade Católica de Brasília
