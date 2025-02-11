# Capítulo 1: A jornada do programa

O objetivo deste livro é ensinar a pensar como um cientista da computação. Esta forma de pensar combina algumas das melhores características da matemática, da engenharia e das ciências naturais. Assim como os matemáticos, os cientistas da computação usam linguagens formais para denotar ideias (especificamente operações de computação). Como engenheiros, eles projetam coisas, reunindo componentes em sistemas e avaliando as opções de melhor retorno entre as alternativas à disposição. Como cientistas, observam o comportamento de sistemas complexos, formam hipóteses e testam previsões.

A habilidade específica mais importante de um cientista da computação é a <a id="termo:resolução de problemas" href="#glos:resolução de problemas">resolução de problemas</a>. Resolução de problemas significa a capacidade de formular problemas, pensar criativamente em soluções e expressar uma solução de forma clara e precisa. Assim, o processo de aprender a programar é uma oportunidade excelente para exercitar a habilidade de resolver problemas. É por isso que este capítulo se chama “A jornada do programa”.

Em um nível você aprenderá a programar, uma habilidade útil por si mesma. Em outro nível usará a programação como um meio para um fim. Conforme avançarmos, este fim ficará mais claro.

## 1.1 - O que é um programa?

Um __programa__ é uma sequência de instruções que especifica como executar uma operação de computação. A operação de computação pode ser algo matemático, como solucionar um sistema de equações ou encontrar as raízes de um polinômio, mas também pode ser uma operação de computação simbólica, como a busca e a substituição de textos em um documento; ou algo gráfico, como o processamento de uma imagem ou a reprodução de um vídeo.

Os detalhes parecem diferentes em linguagens diferentes, mas algumas instruções básicas aparecem em quase todas as linguagens:

<dl>
<dt>entrada</dt>
<dd>Receber dados do teclado, de um arquivo, da rede ou de algum outro dispositivo.</dd>

<dt>saída</dt>
<dd>Exibir dados na tela, salvá-los em um arquivo, enviá-los pela rede etc.</dd>

<dt>matemática</dt>
<dd>Executar operações matemáticas básicas como adição e multiplicação.</dd>

<dt>execução condicional</dt>
<dd>Verificar a existência de certas condições e executar o código adequado.</dd>

<dt>repetição</dt>
<dd>Executar várias vezes alguma ação, normalmente com algumas variações.</dd>
</dl>

Acredite ou não, isto é basicamente tudo o que é preciso saber. Cada programa que você já usou, complicado ou não, é composto de instruções muito parecidas com essas. Podemos então chegar à conclusão de que programar é o processo de quebrar uma tarefa grande e complexa em subtarefas cada vez menores, até que estas sejam simples o suficiente para serem executadas por uma dessas instruções básicas.

## 1.2 - Execução do Python

Um dos desafios de começar a usar Python é ter que instalar no seu computador o próprio programa e outros relacionados. Se tiver familiaridade com o seu sistema operacional, e especialmente se não tiver problemas com a interface de linha de comando, você não terá dificuldade para instalar o Python. Mas para principiantes pode ser trabalhoso aprender sobre administração de sistemas e programação ao mesmo tempo.

Para evitar esse problema, recomendo que comece a executar o Python em um navegador. Depois, quando você já conhecer o Python um pouco mais, darei sugestões para instalá-lo em seu computador.

Há uma série de sites que ajudam a usar e executar o Python. Se já tem um favorito, vá em frente e use-o. Senão, recomendo o PythonAnywhere. Apresento instruções detalhadas sobre os primeiros passos no link http://tinyurl.com/thinkpython2e.

Há duas versões do Python, o Python 2 e o Python 3. Como elas são muito semelhantes, se você aprender uma versão, é fácil trocar para a outra. Como é iniciante, você encontrará poucas diferenças. Este livro foi escrito para o Python 3, mas também incluí algumas notas sobre o Python 2.

O __interpretador__ do Python é um programa que lê e executa o código Python. Dependendo do seu ambiente, é possível iniciar o interpretador clicando em um ícone, ou digitando python em uma linha de comando. Quando ele iniciar, você deverá ver uma saída como esta:

```python
Python 3.4.0 (default, Jun 19 2015, 14:20:21)
[GCC 4.8.2] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```
As três primeiras linhas contêm informações sobre o interpretador e o sistema operacional em que está sendo executado, portanto podem ser diferentes para você. Mas é preciso conferir se o número da versão, que é 3.4.0 neste exemplo, começa com 3, o que indica que você está executando o Python 3. Se começar com 2, você está executando (adivinhe!) o Python 2.

A última linha é um prompt indicando que o interpretador está pronto para você digitar o código. Se digitar uma linha de código e pressionar Enter, o interpretador exibe o resultado:

```python
>>> 1 + 1
2
```
Agora você está pronto para começar. Daqui em diante, vou supor que você sabe como inicializar o interpretador do Python e executar o código.

## 1.3 - O primeiro programa

Tradicionalmente, o primeiro programa que se escreve em uma nova linguagem chama-se “Hello, World!”, porque tudo o que faz é exibir as palavras “Hello, World!” na tela. No Python, ele se parece com isto:

```python
>>> print('Hello, World!')
```

Este é um exemplo de uma instrução print (instrução de impressão), embora na realidade ela não imprima nada em papel. Ela exibe um resultado na tela. Nesse caso, o resultado são as palavras:

```python
Hello, World!
```

As aspas apenas marcam o começo e o fim do texto a ser exibido; elas não aparecem no resultado.

Os parênteses indicam que o print é uma função. Veremos funções no Capítulo 3.

No Python 2, a instrução print é ligeiramente diferente; ela não é uma função, portanto não usa parênteses.

```python
>>> print 'Hello, World!'
```

Esta distinção fará mais sentido em breve, mas isso é o suficiente para começar.

## 1.4 - Operadores aritméticos

Depois do “Hello, World”, o próximo passo é a aritmética. O Python tem operadores, que são símbolos especiais representando operações de computação, como adição e multiplicação.

Os operadores +, - e \* executam a adição, a subtração e a multiplicação, como nos seguintes exemplos:

```python
>>> 40 + 2
42
>>> 43 - 1
42
>>> 6 * 7
42
O operador / executa a divisão:
>>> 84 / 2
42.0
```

Pode ser que você fique intrigado pelo resultado ser 42.0 em vez de 42. Vou explicar isso na próxima seção.

Finalmente, o operador \*\* executa a exponenciação; isto é, eleva um número a uma potência:

```python
>>> 6 ** 2 + 6
42
```

Em algumas outras linguagens, o ^ é usado para a exponenciação, mas no Python é um operador bitwise, chamado XOR. Se não tiver familiaridade com operadores bitwise, o resultado o surpreenderá:

```python
>>> 6 ^ 2
4
```

Não abordarei operadores bitwise neste livro, mas você pode ler sobre eles em http://wiki.python.org/moin/BitwiseOperators.

## 1.5 - Valores e tipos

Um valor é uma das coisas básicas com as quais um programa trabalha, como uma letra ou um número. Alguns valores que vimos até agora foram 2, 42.0 e 'Hello, World!'.

Esses valores pertencem a tipos diferentes: 2 é um número inteiro, 42.0 é um número de ponto flutuante e 'Hello, World!' é uma string, assim chamada porque as letras que contém estão em uma sequência em cadeia.

Se não tiver certeza sobre qual é o tipo de certo valor, o interpretador pode dizer isso a você:

```python
>>> type(2)
<class 'int'>
>>> type(42.0)
<class 'float'>
>>> type('Hello, World!')
<class 'str'>
```

Nesses resultados, a palavra “class” \[classe\] é usada no sentido de categoria; um tipo é uma categoria de valores.

Como se poderia esperar, números inteiros pertencem ao tipo int, strings pertencem ao tipo str e os números de ponto flutuante pertencem ao tipo float.

E valores como '2' e '42.0'? Parecem números, mas estão entre aspas como se fossem strings:

```python
>>> type('2')
<class 'str'>
>>> type('42.0')
<class 'str'>
```

Então são strings.

Ao digitar um número inteiro grande, alguns podem usar a notação americana, com vírgulas entre grupos de dígitos, como em 1,000,000. Este não é um número inteiro legítimo no Python e resultará em:

```python
>>> 1,000,000
(1, 0, 0)
```

O que não é de modo algum o que esperávamos! O Python interpreta 1,000,000 como uma sequência de números inteiros separados por vírgulas. Aprenderemos mais sobre este tipo de sequência mais adiante.

## 1.6 - Linguagens formais e naturais

As linguagens naturais são os idiomas que as pessoas falam, como inglês, espanhol e francês. Elas não foram criadas pelas pessoas (embora as pessoas tentem impor certa ordem a elas); desenvolveram-se naturalmente.

As linguagens formais são linguagens criadas pelas pessoas para aplicações específicas. Por exemplo, a notação que os matemáticos usam é uma linguagem formal especialmente boa para denotar relações entre números e símbolos. Os químicos usam uma linguagem formal para representar a estrutura química de moléculas. E o mais importante:

As linguagens de programação são idiomas formais criados para expressar operações de computação.

As linguagens formais geralmente têm regras de sintaxe estritas que governam a estrutura de declarações. Por exemplo, na matemática a declaração 3 + 3 = 6 tem uma sintaxe correta, mas não 3 + = 3$6. Na química, H2O é uma fórmula sintaticamente correta, mas 2Zz não é.

As regras de sintaxe vêm em duas categorias relativas a símbolos e estrutura. Os símbolos são os elementos básicos da linguagem, como palavras, números e elementos químicos. Um dos problemas com 3 + = 3$6 é que o $ não é um símbolo legítimo na matemática (pelo menos até onde eu sei). De forma similar, 2Zz não é legítimo porque não há nenhum elemento com a abreviatura Zz.

O segundo tipo de regra de sintaxe refere-se ao modo no qual os símbolos são combinados. A equação 3 + = 3 não é legítima porque, embora + e = sejam símbolos legítimos, não se pode ter um na sequência do outro. De forma similar, em uma fórmula química o subscrito vem depois do nome de elemento, não antes.

Esta é um@ frase bem estruturada em portuguê$, mas com s\*mbolos inválidos. Esta frase todos os símbolos válidos tem, mas estrutura válida sem.

Ao ler uma frase em português ou uma declaração em uma linguagem formal, é preciso compreender a estrutura (embora em uma linguagem natural você faça isto de forma subconsciente). Este processo é chamado de análise.

Embora as linguagens formais e naturais tenham muitas características em comum – símbolos, estrutura e sintaxe – há algumas diferenças:

<dl>
<dt>ambiguidade</dt>
<dd>As linguagens naturais são cheias de ambiguidade e as pessoas lidam com isso usando pistas contextuais e outras informações. As linguagens formais são criadas para ser quase ou completamente inequívocas, ou seja, qualquer afirmação tem exatamente um significado, independentemente do contexto.</dd>

<dt>redundância</dt>
<dd>Para compensar a ambiguidade e reduzir equívocos, as linguagens naturais usam muita redundância. Por causa disso, muitas vezes são verborrágicas. As linguagens formais são menos redundantes e mais concisas.</dd>

<dt>literalidade</dt>
<dd>As linguagens naturais são cheias de expressões e metáforas. Se eu digo “Caiu a ficha”, provavelmente não há ficha nenhuma na história, nem nada que tenha caído (esta é uma expressão para dizer que alguém entendeu algo depois de certo período de confusão). As linguagens formais têm significados exatamente iguais ao que expressam.</dd>
</dl>

Como todos nós crescemos falando linguagens naturais, às vezes é difícil se ajustar a linguagens formais. A diferença entre a linguagem natural e a formal é semelhante à diferença entre poesia e prosa, mas vai além:

<dl>
<dt>Poesia</dt>
<dd>As palavras são usadas tanto pelos sons como pelos significados, e o poema inteiro cria um efeito ou resposta emocional. A ambiguidade não é apenas comum, mas muitas vezes proposital.</dd>

<dt>Prosa</dt>
<dd>O significado literal das palavras é o mais importante e a estrutura contribui para este significado. A prosa é mais acessível à análise que a poesia, mas muitas vezes ainda é ambígua.</dd>

<dt>Programas</dt>
<dd>A significado de um programa de computador é inequívoco e literal e pode ser entendido inteiramente pela análise dos símbolos e da estrutura.</dd>
</dl>

As linguagens formais são mais densas que as naturais, então exigem mais tempo para a leitura. Além disso, a estrutura é importante, então nem sempre é melhor ler de cima para baixo e da esquerda para a direita. Em vez disso, aprenda a analisar o programa primeiro, identificando os símbolos e interpretando a estrutura. E os detalhes fazem diferença. Pequenos erros em ortografia e pontuação, que podem não importar tanto nas linguagens naturais, podem fazer uma grande diferença em uma língua formal.

## 1.7 - Depuração

Os programadores erram. Por um capricho do destino, erros de programação são chamados de bugs (insetos) e o processo de rastreá-los chama-se depuração (debugging).

Programar, e especialmente fazer a depuração, às vezes traz emoções fortes. Se tiver dificuldade com certo bug, você pode ficar zangado, desesperado ou constrangido.

Há evidências de que as pessoas respondem naturalmente a computadores como se fossem pessoas. Quando funcionam bem, pensamos neles como parceiros da equipe, e quando são teimosos ou grosseiros, respondemos a eles do mesmo jeito que fazemos com pessoas grosseiras e teimosas (Reeves e Nass, [_The Media Equation: How People Treat Computers, Television, and New Media Like Real People and Places_](https://en.wikipedia.org/wiki/The_Media_Equation) — _A equação da mídia: como as pessoas tratam os computadores, a televisão e as novas mídias como se fossem pessoas e lugares reais_).

Prepare-se para essas reações, pois isso pode ajudar a lidar com elas. Uma abordagem é pensar no computador como um funcionário com certas vantagens, como velocidade e precisão, e certas desvantagens, como a falta de empatia e a incapacidade de compreender um contexto mais amplo.

Seu trabalho é ser um bom gerente: encontrar formas de aproveitar as vantagens e atenuar as desvantagens. E também encontrar formas de usar suas emoções para lidar com o problema sem deixar suas reações interferirem na sua capacidade de trabalho.

Aprender a depurar erros pode ser frustrante, mas é uma habilidade valiosa, útil para muitas atividades além da programação. No fim de cada capítulo há uma seção como esta, com as minhas sugestões para fazer a depuração. Espero que sejam úteis!

## 1.8 - Glossário

<dl>
<dt><a id="glos:resolução de problemas" href="#termo:resolução de problemas">resolução de problemas</a></dt>
<dd>O processo de formular um problema, encontrar uma solução e expressá-la.</dd>

<dt><a id="glos:linguagem de alto nível" href="#termo:linguagem de alto nível">linguagem de alto nível</a></dt>
<dd>Uma linguagem de programação como Python, que foi criada com o intuito de ser fácil para os humanos escreverem e lerem.</dd>

<dt><a id="glos:linguagem de baixo nível" href="#termo:linguagem de baixo nível">linguagem de baixo nível</a></dt>
<dd>Uma linguagem de programação criada para o computador executar com facilidade; também chamada de “linguagem de máquina” ou “linguagem assembly”.</dd>

<dt><a id="glos:portabilidade" href="#termo:portabilidade">portabilidade</a></dt>
<dd>A propriedade de um programa de poder ser executado em mais de um tipo de computador.</dd>

<dt><a id="glos:interpretador" href="#termo:interpretador">interpretador</a></dt>
<dd>Um programa que lê outro programa e o executa.</dd>

<dt><a id="glos:prompt" href="#termo:prompt">prompt</a></dt>
<dd>Caracteres expostos pelo interpretador para indicar que está pronto para receber entradas do usuário.<br>
<em>No console interativo do Python costuma ser:</em> <code> >>> </code></dd>


<dt><a id="glos:programa" href="#termo:programa">programa</a></dt>
<dd>Conjunto de instruções que especificam uma operação de computação.</dd>

<dt><a id="glos:instrução print" href="#termo:instrução print">instrução print</a></dt>
<dd>Uma instrução que faz o interpretador do Python exibir um valor na tela. </br><i>Note que no Python 3 trata-se de uma função que deve ser chamada com parenteses: <code>print(valor)</code>.</i></dd>

<dt><a id="glos:operador" href="#termo:operador">operador</a></dt>
<dd>Um símbolo especial que representa uma operação de computação simples como adição (<code>+</code>), multiplicação (<code>*</code>) ou concatenação de strings (<em>também o </em><code>+</code>).</dd>

<dt><a id="glos:valor" href="#termo:valor">valor</a></dt>
<dd>Uma das unidades básicas de dados, como um número ou string (<em>sequencias de caracteres, texto</em>), que um programa manipula.</dd>

<dt><a id="glos:tipo" href="#termo:tipo">tipo</a></dt>
<dd>Uma categoria de valores. Os tipos que vimos por enquanto são números inteiros (tipo <code>int</code>), números de ponto flutuante (tipo <code>float</code>) e strings (tipo <code>str</code>).</dd>

<dt><a id="glos:inteiro" href="#termo:inteiro">inteiro</a></dt>
  <dd>Um tipo que representa números inteiros. <em>Exemplos: <code>42</code> , <code>0</code>, ou <code>-100</code>.</em></dd>

<dt><a id="glos:ponto flutuante" href="#termo:ponto flutuante">ponto flutuante</a></dt>
<dd>Um tipo que representa números com partes fracionárias.<br>
    <em>No Brasil, em português, o separador decimal é a vírgula, mas na maior parte das linguagens de programação, com influência da língua inglesa, o separador decimal é o ponto, então representação decimal dos números de ponto flutuante, floating point, (abreviadamente float) é com ponto. Exemplos: <code>3.14</code>, ou <code>0.23</code>.</em></dd>

<dt><a id="glos:string" href="#termo:string">string</a></dt>
<dd>Um tipo que representa sequências de caracteres.<br>
  <em>No corpo do programa podemos criar strings com expressões entre aspas, exemplo:</em> <code>nome = 'Alexandre'</code>. <em>A variável nome agora aponta para um string. Mas futuramente veremos que dados em forma de string podem vir de fontes fora do programa também.</em></dd>

<dt><a id="glos:linguagem natural" href="#termo:linguagem natural">linguagem natural</a></dt>
<dd>Qualquer linguagem que as pessoas falam e que se desenvolveu naturalmente.</dd>

<dt><a id="glos:linguagem formal" href="#termo:linguagem formal">linguagem formal</a></dt>
<dd>Qualquer linguagem que as pessoas criaram com objetivos específicos, como representar ideias matemáticas ou programas de computador; todas as linguagens de programação são linguagens formais.</dd>

<dt><a id="glos:símbolo" href="#termo:símbolo">símbolo</a></dt>
<dd>Um dos elementos básicos da estrutura sintática de um programa, análogo a uma palavra em linguagem natural.</dd>

<dt><a id="glos:sintaxe" href="#termo:sintaxe">sintaxe</a></dt>
<dd>As regras que governam a estrutura de um programa.</dd>

<dt><a id="glos:análise" href="#termo:análise">análise</a></dt>
<dd>Examinar um programa e sua estrutura sintática.</dd>

<dt><a id="glos:bug" href="#termo:bug">bug</a></dt>
<dd>Um erro em um programa.</dd>

<dt><a id="glos:depuração" href="#termo:depuração">depuração</a></dt>
<dd>O processo de encontrar e corrigir (depurar) bugs. <em>As pessoas também falam "debugar"</em></dd>
</dl>

## 1.9 - Exercícios

### Exercício 1.1

É uma boa ideia ler este livro em frente a um computador para testar os exemplos durante a leitura.

Sempre que estiver testando um novo recurso, você deve tentar fazer erros. Por exemplo, no programa “Hello, World!”, o que acontece se omitir uma das aspas? E se omitir ambas? E se você soletrar a instrução print de forma errada?

Este tipo de experimento ajuda a lembrar o que foi lido; também ajuda quando você estiver programando, porque assim conhecerá o significado das mensagens de erro. É melhor fazer erros agora e de propósito que depois e acidentalmente.

1. Em uma instrução print, o que acontece se você omitir um dos parênteses ou ambos?

2. Se estiver tentando imprimir uma string, o que acontece se omitir uma das aspas ou ambas?

3. Você pode usar um sinal de menos para fazer um número negativo como -2. O que acontece se puser um sinal de mais antes de um número? E se escrever assim: 2++2?

4. Na notação matemática, zeros à esquerda são aceitáveis, como em 02. O que acontece se você tentar usar isso no Python?

5. O que acontece se você tiver dois valores sem nenhum operador entre eles?

### Exercício 1.2

Inicialize o interpretador do Python e use-o como uma calculadora.

1. Quantos segundos há em 42 minutos e 42 segundos?

2. Quantas milhas há em 10 quilômetros? Dica: uma milha equivale a 1,61 quilômetro.

3. Se você correr 10 quilômetros em 42 minutos e 42 segundos, qual é o seu passo médio (tempo por milha em minutos e segundos)? Qual é a sua velocidade média em milhas por hora?
