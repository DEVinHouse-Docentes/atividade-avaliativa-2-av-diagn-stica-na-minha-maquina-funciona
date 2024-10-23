# Avaliação Diagnóstica - Prova Objetiva - Lógica de Programação com Java

## Introdução e contextualização

Esta avaliação diagnóstica visa identificar o conhecimento prévio dos alunos em Lógica de Programação com Java, como base para o desenvolvimento das capacidades da UC de Programação de Aplicativos fortemente alicerçada em Programação Orientada a Objetos (POO). As questões foram elaboradas considerando os níveis cognitivos da Taxonomia de Bloom e os requisitos técnicos para construção de itens de múltipla escolha.

## Justificativa
A MSEP, na p.152, declara o objetivo da avaliação diagnóstica, como se segue:
> ... na execução dos cursos, o Docente deve sondar os conhecimentos prévios dos Alunos, por meio de uma avaliação diagnóstica, visando alinhar a sua prática às características dos Alunos. Nesse sentido, a avaliação diagnóstica objetiva: <br>
Verificar se os Alunos dispõem dos pré-requisitos necessários para o desenvolvimento das capacidades previstas na unidade curricular;<br>
Adotar estratégias para nivelamento de conhecimentos, caso seja constatada a ausência de pré-requisitos para o desenvolvimento das capacidades da unidade curricular; <br>
Flexibilizar as ações planejadas para atender às necessidades individuais de aprendizagem dos Alunos;<br>
Levantar expectativas e interesses dos Alunos para, na medida do possível, contemplá-las ao longo do processo de ensino, visando a promoção de aprendizagens significativas.

Com relação à escolha do instrumento de avaliação, a saber, Prova Objetiva, a MSEP, na p. 128, define que:
> **Provas objetivas**: são estruturadas por meio de itens de avaliação que visam mapear pontualmente os diferentes aspectos de uma capacidade. Devem ser construídas de modo contextualizado, evitando apenas a memorização e apresentando situações possíveis de serem enfrentadas pelo Aluno. Caracterizam-se por propor que o Aluno identifque, dentre múltiplas escolhas, qual alternativa melhor responde ao que está sendo arguido, sendo uma delas a correta e as demais distratores, ou seja, possibilidades incorretas do ponto de vista da capacidade avaliada, mas plausíveis em outros contextos. Este tipo de instrumento é mais apropriado para investigação do domínio cognitivo.

Tendo em vista que os conhecimentos em Lógica de Programação com Java, são ministrado no primeiro semestre, os níveis da Taxonomia de Bloom que serão utilizados para a elaboração das questões serão `LEMBRAR`, `ENTENDER` e `APLICAR`. Ressalta-se, que apesar do verbo `APLICAR` estar em um nível elevado da Taxonomia, ele será usado em concordância com os níveis de `LEMBRAR` e `ENTENDER`, ou seja, o aluno irá aplicar por lembrar ou entender o conceito/fundamento avaliado.

Quanto a elaboração de itens avaliativos:
1. Segui a estrutura recomendada para cada item: contexto, comando e cinco alternativas (incluindo o gabarito e quatro distratores).
2. Criei contextos relevantes para a área de programação, aproximando-se de situações que os alunos podem encontrar em sua futura prática profissional.
3. Formulei comandos claros e objetivos, evitando expressões proibidas e sentenças negativas, com verbos adequados ao nível da Taxonomia de Bloom.
4. Elaborei alternativas plausíveis, todas justificadas, tanto a correta como os distratores.
5. Evitei "pegadinhas" ou questões que exigissem simples memorização de números ou fórmulas.
6. Mantive uma linguagem clara, objetiva e técnica, apropriada para o nível dos alunos.
7. Certifiquei-me de que cada **Questão** aborda apenas uma capacidade e pode ser respondida em aproximadamente 3 minutos.

Esses pontos estão de acordo com o Manual de Elaboração de Itens do SisBia, pp. 39-53

## Protótipo da Avaliação
Poderia ser criada como Avaliação no AVA Moodle ou como formulário no Google Forms. 
### Questões

#### **Questão** 1 (Nível: Lembrar)

**Contexto:**
Em um projeto de desenvolvimento de software, é fundamental compreender os conceitos básicos da linguagem Java para codificar algoritmos eficientes.

**Comando:**
Identifique a afirmação correta sobre os tipos de dados primitivos em Java.

**Alternativas:**

a) O tipo `float` ocupa mais espaço na memória que o tipo `double`.

b) O tipo `char` pode armazenar múltiplos caracteres em uma única variável.

c) O tipo `boolean` pode armazenar os valores `true`, `false` ou `null`.

d) O tipo `int` pode armazenar números inteiros na faixa de -2³¹ a 2³¹-1.

e) O tipo `byte` é capaz de armazenar valores decimais com precisão de 8 casas.

**Gabarito:** d

**Justificativas:**

a) Incorreta. O tipo `double` ocupa 64 bits, enquanto `float` ocupa 32 bits.

b) Incorreta. O tipo `char` armazena apenas um único caractere Unicode.

c) Incorreta. O tipo `boolean` armazena apenas `true` ou `false`, não `null`.

d) Correta. O tipo `int` em Java é um inteiro de 32 bits com sinal, armazenando valores de -2³¹ a 2³¹-1.

e) Incorreta. O tipo `byte` é um inteiro de 8 bits, não armazena valores decimais.

#### **Questão** 2 (Nível: Entender)

**Contexto:**
Durante o desenvolvimento de um sistema de controle de estoque, um programador precisa implementar uma estrutura de repetição para processar uma lista de produtos.

**Comando:**
Observe o trecho de código abaixo e identifique sua funcionalidade.

```java
for (int i = 0; i < produtos.length; i += 2) {
    System.out.println(produtos[i]);
}
```

**Alternativas:**

a) Imprime todos os elementos do array `produtos`.

b) Imprime os elementos do array `produtos` em ordem reversa.

c) Imprime apenas os elementos de índice par do array `produtos`.

d) Imprime os elementos do array `produtos` duas vezes.

e) Gera um erro de compilação devido ao incremento inadequado.

**Gabarito:** c

**Justificativas:**

a) Incorreta. O loop não imprime todos os elementos, apenas os de índice par.

b) Incorreta. O loop percorre o array na ordem normal, não reversa.

c) Correta. O incremento `i += 2` faz com que apenas os elementos de índice par sejam acessados e impressos.

d) Incorreta. Cada elemento é impresso apenas uma vez, se for de índice par.

e) Incorreta. O código é válido e não gera erro de compilação.

#### **Questão** 3 (Nível: Aplicar ao Recordar)

**Contexto:**
Em um sistema de gerenciamento de biblioteca, é necessário implementar uma função para verificar se um número de identificação de livro é válido. Um número é considerado válido se for par e divisível por 3.

**Comando:**
Indique o trecho de código que implementa corretamente a função de validação do número de identificação do livro.

**Alternativas:**

a) 
```java
public boolean isValidId(int id) {
    return id % 2 == 0 || id % 3 == 0;
}
```
b)
```java
public boolean isValidId(int id) {
    return id % 2 == 0 && id % 3 == 0;
}
```
c)
```java
public boolean isValidId(int id) {
    return (id % 2 == 0) ? (id % 3 == 0) : false;
}
```
d)
```java
public boolean isValidId(int id) {
    if (id % 2 == 0) {
        return id % 3 == 0;
    }
    return false;
}
```


**Gabarito:** b

**Justificativas:**

a) Incorreta. Esta função retorna true se o número for par OU divisível por 3, não ambos.

b) Correta. Esta função verifica corretamente se o número é par E divisível por 3.

c) Incorreta. Apesar de funcional, esta implementação é desnecessariamente complexa.

d) Incorreta. Embora funcional, esta implementação é menos eficiente e clara que a alternativa b.


#### **Questão** 4 (Nível: Entender)

**Contexto:**
Em um sistema de gerenciamento de vendas, é necessário calcular o desconto aplicado a um produto com base em seu preço. O sistema utiliza uma estrutura condicional para determinar o percentual de desconto.

**Comando:**
Observe o código abaixo e identifique qual será o desconto aplicado a um produto com preço de R$ 150,00.

```java
public double calcularDesconto(double preco) {
    double desconto;
    if (preco < 100) {
        desconto = 0.05;
    } else if (preco < 200) {
        desconto = 0.10;
    } else if (preco < 300) {
        desconto = 0.15;
    } else {
        desconto = 0.20;
    }
    return preco * desconto;
}
```

**Alternativas:**

a) R$ 7,50

b) R$ 15,00

c) R$ 22,50

d) R$ 30,00


**Gabarito:** b

**Justificativas:**

a) Incorreta. Este seria o desconto se o percentual fosse 5% (preço < 100).

b) Correta. Para um preço de R$ 150,00, o desconto é de 10% (0.10), resultando em R$ 15,00.

c) Incorreta. Este seria o desconto se o percentual fosse 15% (200 <= preço < 300).

d) Incorreta. Este seria o desconto se o percentual fosse 20% (preço >= 300).


#### **Questão** 5 (Nível: Aplicar ao Entender)

**Contexto:**
Uma empresa de análise de dados precisa implementar um algoritmo para calcular a média móvel de um conjunto de valores. A média móvel é calculada como a média dos últimos N valores de uma série.

**Comando:**
Selecione o trecho de código que implementa corretamente o cálculo da média móvel para os últimos 3 valores de um array.

**Alternativas:**

a)
```java
public double calcularMediaMovel(double[] valores) {
    double soma = 0;
    for (int i = 0; i < 3; i++) {
        soma += valores[i];
    }
    return soma / 3;
}
```
b)
```java
public double calcularMediaMovel(double[] valores) {
    double soma = 0;
    for (int i = valores.length - 3; i < valores.length; i++) {
        soma += valores[i];
    }
    return soma / 3;
}
```
c)
```java
public double calcularMediaMovel(double[] valores) {
    double soma = valores[valores.length - 1] + valores[valores.length - 2] + valores[valores.length - 3];
    return soma / 3;
}
```
d)
```java
public double calcularMediaMovel(double[] valores) {
    double soma = 0;
    for (double valor : valores) {
        soma += valor;
    }
    return soma / 3;
}
```


**Gabarito:** b

**Justificativas:**

a) Incorreta. Calcula a média dos primeiros 3 valores, não dos últimos.

b) Correta. Calcula corretamente a média dos últimos 3 valores do array.

c) Incorreta. Funciona, mas é menos flexível e mais propensa a erros que a solução b.

d) Incorreta. Calcula a média de todos os valores do array, não apenas dos últimos 3.


#### **Questão** 6 (Nível: Lembrar)

**Contexto:**
Durante o desenvolvimento de um sistema de cadastro, um programador precisa implementar uma estrutura para armazenar uma lista de nomes de usuários.

**Comando:**
Identifique a declaração correta para criar um array de strings capaz de armazenar 10 nomes de usuários em Java.

**Alternativas:**

a) `String nomes = new String[10];`

b) `String[] nomes = new String[10];`

c) `String nomes[] = new String[];`

d) `String[] nomes = new String[10][];`


**Gabarito:** b

**Justificativas:**

a) Incorreta. Esta sintaxe declara uma única variável String, não um array.

b) Correta. Esta é a sintaxe correta para declarar um array de strings com 10 elementos.

c) Incorreta. Falta especificar o tamanho do array na criação.

d) Incorreta. Esta sintaxe cria um array bidimensional, não um array unidimensional de strings.


#### **Questão** 7 (Nível: Aplicar ao Entender)

**Contexto:**
Uma empresa de e-commerce precisa implementar um sistema de classificação de produtos com base nas avaliações dos clientes. As avaliações são armazenadas em um array de inteiros, onde cada elemento representa a nota dada por um cliente (de 1 a 5 estrelas).

**Comando:**
Selecione o trecho de código que calcula corretamente a média das avaliações, arredondando o resultado para o inteiro mais próximo.

**Alternativas:**

a)
```java
public int calcularMediaAvaliacoes(int[] avaliacoes) {
    int soma = 0;
    for (int avaliacao : avaliacoes) {
        soma += avaliacao;
    }
    return soma / avaliacoes.length;
}
```
b)
```java
public int calcularMediaAvaliacoes(int[] avaliacoes) {
    double soma = 0;
    for (int avaliacao : avaliacoes) {
        soma += avaliacao;
    }
    return (int) Math.round(soma / avaliacoes.length);
}
```
c)
```java
public int calcularMediaAvaliacoes(int[] avaliacoes) {
    int soma = 0;
    for (int avaliacao : avaliacoes) {
        soma += avaliacao;
    }
    return Math.round(soma / avaliacoes.length);
}
```
d)
```java
public int calcularMediaAvaliacoes(int[] avaliacoes) {
    double soma = 0;
    for (int avaliacao : avaliacoes) {
        soma += avaliacao;
    }
    return (int) (soma / avaliacoes.length + 0.5);
}
```


**Gabarito:** b

**Justificativas:**

a) Incorreta. Realiza divisão inteira, truncando o resultado sem arredondar.

b) Correta. Calcula a média como double e usa Math.round para arredondar corretamente.

c) Incorreta. Causa erro de compilação, pois Math.round(float) retorna long, não int.

d) Incorreta. Implementa arredondamento manual, mas pode falhar para alguns casos.


#### **Questão** 8 (Nível: Entender)

**Contexto:**
Um desenvolvedor está criando um jogo de RPG e precisa implementar um sistema de níveis para os personagens. O nível do personagem é determinado pela quantidade de pontos de experiência (XP) acumulados.

**Comando:**
Observe o código abaixo e indique qual será o nível de um personagem com 7500 pontos de experiência.

```java
public int calcularNivel(int xp) {
    if (xp < 1000) return 1;
    if (xp < 3000) return 2;
    if (xp < 6000) return 3;
    if (xp < 10000) return 4;
    return 5;
}
```

**Alternativas:**

a) 1

b) 2

c) 3

d) 4


**Gabarito:** d

**Justificativas:**

a) Incorreta. Nível 1 é para XP menor que 1000.

b) Incorreta. Nível 2 é para XP entre 1000 e 2999.

c) Incorreta. Nível 3 é para XP entre 3000 e 5999.

d) Correta. Para 7500 XP, o nível é 4 (6000 <= XP < 10000).


#### **Questão** 9 (Nível: Lembrar)

**Contexto:**
Durante uma revisão de código em um projeto de software, um programador júnior precisa identificar o uso correto de operadores lógicos em Java.

**Comando:**
Identifique a expressão que corretamente verifica se uma variável inteira 'idade' está no intervalo de 18 a 65 anos, inclusive.

**Alternativas:**

a) `idade >= 18 && idade <= 65`

b) `idade > 18 || idade < 65`

c) `!(idade < 18) || !(idade > 65)`

d) `idade => 18 && idade =< 65`


**Gabarito:** a

**Justificativas:**

a) Correta. Verifica corretamente se idade é maior ou igual a 18 E menor ou igual a 65.

b) Incorreta. Esta expressão é verdadeira para qualquer idade, exceto 18 e 65.

c) Incorreta. Embora logicamente equivalente, é desnecessariamente complexa e menos legível.

d) Incorreta. Usa operadores de comparação inválidos em Java (=> e =<).


#### **Questão** 10 (Nível: Aplicar ao Entender)

**Contexto:**
Uma equipe de desenvolvimento está criando um sistema de controle de acesso para uma empresa. O sistema precisa verificar se uma senha fornecida pelo usuário atende aos critérios de segurança estabelecidos.

**Comando:**
Selecione o trecho de código que verifica corretamente se uma senha tem pelo menos 8 caracteres, contém pelo menos uma letra maiúscula e um número.

**Alternativas:**

a)
```java
public boolean senhaValida(String senha) {
    return senha.length() >= 8 && senha.matches(".*[A-Z].*") && senha.matches(".*[0-9].*");
}
```
b)
```java
public boolean senhaValida(String senha) {
    return senha.length() >= 8 && senha.contains("[A-Z]") && senha.contains("[0-9]");
}
```
c)
```java
public boolean senhaValida(String senha) {
    boolean temMaiuscula = false;
    boolean temNumero = false;
    for (char c : senha.toCharArray()) {
        if (Character.isUpperCase(c)) temMaiuscula = true;
        if (Character.isDigit(c)) temNumero = true;
    }
    return senha.length() >= 8 && temMaiuscula && temNumero;
}
```
d)
```java
public boolean senhaValida(String senha) {
    return senha.matches("^(?=.*[A-Z])(?=.*[0-9]).{8,}$");
}
```


**Gabarito:** d

**Justificativas:**

a) Incorreta. Usa regex corretamente para maiúsculas e números, mas de forma ineficiente.

b) Incorreta. O método contains() não aceita regex, então não funcionará como esperado.

c) Incorreta. Funciona, mas é mais verbosa e potencialmente menos eficiente que outras soluções.

d) Correta. Usa uma única expressão regular para verificar todos os critérios eficientemente.


---

**Questão 11 (Nível: Lembrar)**  

**Contexto:** Durante o desenvolvimento de uma aplicação bancária, você precisa manipular valores monetários para calcular saldo e outras operações. Para isso, é necessário entender os tipos de dados apropriados.

**Comando:** Identifique o tipo de dado correto para representar valores monetários com precisão em Java.

**Alternativas:**

a) `int`  

b) `boolean`  

c) `double`  

d) `char`  

e) `byte`

**Gabarito:** c

**Justificativas:**

a) Incorreta. O tipo `int` armazena apenas números inteiros e não é adequado para valores monetários que podem ter casas decimais.  

b) Incorreta. O tipo `boolean` armazena apenas valores lógicos (true/false).  

c) Correta. O tipo `double` é comumente usado para representar números com casas decimais, como valores monetários.  

d) Incorreta. O tipo `char` armazena caracteres, não valores numéricos.  

e) Incorreta. O tipo `byte` é um tipo de dado numérico, mas armazena apenas inteiros pequenos e não suporta casas decimais.

---

**Questão 12 (Nível: Entender)**  

**Contexto:** Um desenvolvedor está criando um sistema para calcular o total de vendas de uma loja online. O programa deve somar o preço de cada produto no carrinho de compras.

**Comando:** Observe o código abaixo e identifique sua funcionalidade.

```java
double total = 0;
for (int i = 0; i < produtos.length; i++) {
    total += produtos[i].preco;
}
```

**Alternativas:**

a) Calcula o preço total de todos os produtos no array `produtos`.  

b) Calcula a média do preço dos produtos no array `produtos`. 

c) Calcula o número de produtos no array `produtos`.  

d) Verifica se todos os produtos no array `produtos` têm o mesmo preço.  

e) Imprime o preço de cada produto no array `produtos`.

**Gabarito:** a

**Justificativas:**

a) Correta. O laço `for` percorre todos os produtos e soma seus preços na variável `total`.  

b) Incorreta. O código apenas soma os preços, não calcula a média.  

c) Incorreta. O código não conta o número de produtos, apenas soma seus preços.  

d) Incorreta. O código não verifica se os preços são iguais, apenas os soma.  

e) Incorreta. O código não imprime os preços, ele apenas os soma na variável `total`.

---

**Questão 13 (Nível: Aplicar ao Recordar)**  

**Contexto:** Uma empresa de tecnologia está desenvolvendo um software que calcula o tempo total de uso de máquinas em uma fábrica. O programa precisa armazenar e exibir o tempo em horas, minutos e segundos.

**Comando:** Indique o código que armazena corretamente o tempo total de uso em três variáveis: horas, minutos e segundos.

**Alternativas:**

a) `int horas, minutos, segundos;`  

b) `double horas, minutos, segundos;`  

c) `boolean horas, minutos, segundos;`  

d) `String horas, minutos, segundos;`  

e) `char horas, minutos, segundos;`

**Gabarito:** a

**Justificativas:**

a) Correta. O tipo `int` é o mais adequado para armazenar horas, minutos e segundos, pois são valores inteiros.  

b) Incorreta. O tipo `double` armazena números com casas decimais, o que não é necessário para horas, minutos e segundos.  

c) Incorreta. O tipo `boolean` armazena apenas valores lógicos (true/false).  

d) Incorreta. O tipo `String` armazena texto, não números.  

e) Incorreta. O tipo `char` armazena caracteres individuais, o que não é adequado para representar tempo.

---

**Questão 14 (Nível: Lembrar)**  

**Contexto:** Em um projeto de desenvolvimento de software, é fundamental entender como utilizar estruturas de controle para controlar o fluxo de execução de um programa.

**Comando:** Identifique a alternativa que apresenta um exemplo correto de uma estrutura condicional em Java.

**Alternativas:**

a) `if (x > 10) { System.out.println("Maior que 10"); }`  

b) `if [x > 10] { System.out.println("Maior que 10"); }`  

c) `if x > 10 { System.out.println("Maior que 10"); }`  

d) `if (x > 10) System.out.println("Maior que 10")`  

e) `if (x > 10) { System.out.println("Maior que 10")`

**Gabarito:** a

**Justificativas:**

a) Correta. Esta é a sintaxe correta de uma estrutura condicional em Java, com parênteses em torno da condição e chaves para o bloco de código.  

b) Incorreta. A estrutura condicional em Java usa parênteses, não colchetes.  

c) Incorreta. A condição precisa estar entre parênteses em Java.  

d) Incorreta. Faltam as chaves no bloco de código, e a linha não termina com ponto e vírgula.  

e) Incorreta. Faltam os pontos e vírgulas após as instruções dentro do bloco de código.

---

**Questão 15 (Nível: Aplicar ao Recordar)**  

**Contexto:** Em uma aplicação de gerenciamento de pedidos, é necessário verificar se o valor total de um pedido excede um valor determinado para aplicar um desconto especial.

**Comando:** Indique o trecho de código que aplica corretamente um desconto de 15% ao valor total de um pedido se ele for maior que R$ 500,00.

**Alternativas:**

a) `if (valorTotal > 500) { valorTotal = valorTotal - (valorTotal * 0.15); }`  

b) `if (valorTotal > 500) { valorTotal = valorTotal + (valorTotal * 0.15); }`  

c) `if (valorTotal > 500) { valorTotal = valorTotal / 0.85; }`  

d) `if (valorTotal > 500) { valorTotal = valorTotal - 0.15; }`  

e) `if (valorTotal > 500) { valorTotal = valorTotal * 1.15; }`

**Gabarito:** a

**Justificativas:**

a) Correta. O código calcula 15% do valor total e subtrai este valor para aplicar o desconto.  

b) Incorreta. Somar 15% ao valor total aumentaria o valor em vez de aplicar o desconto.  

c) Incorreta. Dividir o valor total por 0.85 aumentaria o valor em vez de aplicar o desconto.  

d) Incorreta. Subtrair 0.15 diretamente não aplicaria o desconto corretamente.  

e) Incorreta. Multiplicar o valor por 1.15 aumentaria o valor total em 15%, em vez de aplicar o desconto.

---

Essas novas questões seguem o padrão solicitado, com contextos práticos relacionados ao uso de **Java** em situações profissionais, mantendo a coerência com os níveis da **Taxonomia de Bloom** (Lembrar, Entender e Aplicar ao Recordar).
