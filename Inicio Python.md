\*\* Inicio da Jornada \*\*



Funções Python



print()



print(): A função print exibe informações na tela. Os valores que queremos mostrar são colocados entre os parênteses. textos (string) devem ficar entre aspas simples('') ou aspas duplas ("").



EXEMPLO:



print('Nutella lindo')

print(7)



para escrever a sequencia (Nutella 7 anos) o print deve seguir a regra das asas e virgula



EXEMPLO:



print('nutella',7,'anos')





type()



A função type() mostra o tipo de um valor ou de uma variável.



EXEMPLO:



print(type(10))

print(type("Pedro"))



RESULTADO:

<class 'int'>

<class 'str'>



Int -> números inteiros (1, 10, 100)

Float -> números com casas decimais (3.1, 9.1)

Str -> Textos (string)

Bool = True ou False



Type é usado para definir o tipo do dado da variável, as variáveis são como caixas que armazenam valores.



EXEMPLOS:



Nome = 'Nutella'

Idade = 7



Nome é a variável (caixa) e Nutella é o valor guardado na caixa.



Idade é a Variável e 7 é valor armazenado



FUNÇÕES PARA STRINGS



str.upper() : deixa o texto (string) em letras maiúsculas.

str.lower() : deixa o texto (string) em letras minúsculas.

str.strip() : remove os espaços em branco no início e no final de uma string.

str.replace("antigo", "novo") : substitui todas as ocorrências de um texto por outro dentro da string.



Coletando dados



Através da função input() conseguimos coletar dados da pessoa usuária. Para armazenar o valor digitado, é necessário atribuí-lo a uma variável.



EXEMPLO:



nome = input("Digite seu nome: ")



O valor retornado por input() é sempre do tipo string (str), mesmo quando a pessoa digita números.



Para converter o valor para outros tipos de dados, podemos usar:



Inteiro: int(input())

Decimal: float(input())



\# ESTRUTURAS CONDICIONAIS



\## If



`if` significa \*\*"se"\*\*. É utilizado para verificar se uma condição é verdadeira e executar um bloco de código quando isso acontece.



\## Else



`else` significa \*\*"senão"\*\*. É utilizado junto com o `if` e será executado quando a condição do `if` for avaliada como \*\*False\*\*.



\### Exemplo de sintaxe



```python

if condição:

&#x20;   # código executado se a condição for verdadeira

else:

&#x20;   # código executado se a condição for falsa

```



## Exemplo



```python

media = float(input("Digite a média: "))



if media >= 6.0:

&#x20;   print("Aprovado")

else:

&#x20;   print("Reprovado")

```



Neste exemplo:



\* Se a média for maior ou igual a 6.0, a pessoa será aprovada.

\* Se a média for menor que 6.0, a pessoa será reprovada.



\---

\##\*\*Operadores de Comparação\*\*



==	igual a



!=	diferente de



>	maior que



<	menor que



>=	maior ou igual a



<=	menor ou igual a





\## Elif



`elif` é a junção de \*\*else + if\*\* e significa \*\*"senão, se"\*\*.



Ele permite verificar várias condições em sequência. Caso a condição do `if` seja falsa, o Python verificará a condição do primeiro `elif`, depois do segundo e assim por diante.



Se nenhuma condição for verdadeira, o bloco `else` será executado.



\### Exemplo de sintaxe



```python

if condição1:

&#x20;   # faça algo

elif condição2:

&#x20;   # faça outra coisa

elif condição3:

&#x20;   # faça mais alguma coisa

else:

&#x20;   # faça algo diferente

```



\### Exemplo



```python

nota = 8



if nota >= 9:

&#x20;   print("Excelente")

elif nota >= 6:

&#x20;   print("Aprovado")

else:

&#x20;   print("Reprovado")

```



\---



\# OPERADORES LÓGICOS



\## And (E)



Use quando \*\*todas as condições precisam ser verdadeiras\*\*.



```python

if idade >= 16 and tem\_titulo:

&#x20;   print("Pode votar")

else:

&#x20;   print("Não pode votar")

```



\---



\## Or (OU)



Use quando \*\*pelo menos uma condição precisa ser verdadeira\*\*.



```python

if estudante or idoso:

&#x20;   print("Tem desconto")

```



\---



\## Not (NÃO)



Use para inverter um valor lógico.



```python

if not logado:

&#x20;   print("Acesso bloqueado")

```



\### Dica



Quando o enunciado utilizar as palavras:



\* \*\*e\*\* → geralmente usamos `and`

\* \*\*ou\*\* → geralmente usamos `or`

\* \*\*não\*\* → geralmente usamos `not`



\---



\# OPERADOR IN



\## In



O operador `in` é utilizado para verificar se um elemento está presente em uma lista, tupla, string ou outro conjunto de dados.



\### Exemplo



```python

nome = "José"



lista\_festa = \[

&#x20;   "Lucas",

&#x20;   "Luiggi",

&#x20;   "Luan",

&#x20;   "Enrique",

&#x20;   "Pedro",

&#x20;   "Barbosa",

&#x20;   "Gustavo",

&#x20;   "Luiz",

&#x20;   "Felipe",

&#x20;   "Matheus"

]



if nome in lista\_festa:

&#x20;   print("Nome está na lista")

else:

&#x20;   print("Nome não está na lista")

```



\### Outro exemplo



```python

letra = "a"



if letra in "banana":

&#x20;   print("A letra existe na palavra")

```



O operador `in` sempre responde à pergunta:



\*\*"Esse elemento está dentro desse conjunto?"\*\*





\##\*\*Estrutura de Repetição\*\*



While : O laço While é uma estrutura de repetição em python que permite executar um bloco de código repetidamente enquanto uma determinada condição é verdadeira:



ESTRUTURA:



while condição:

&#x20;  #bloco de código 



EXEMPLO



contador = 1 

while contador <= 10:

&#x09;print(contador)

&#x09;contador = contador + 1



For : O laço for é um tipo de estrutura de controle de fluxo que permite interar sobre um conjunto de elementos



ESTRUTURA:



for elemento in conjunto:

&#x09;# código a ser executado para cada elemento



for numero in range(1, 6):

&#x20;   print(numero)



\*\*IMPORTANTE\*\* 



O for pode ser utilizado com a função range(), essa função gera uma sequencia de numero inteiros a partir do parâmetro inicio até o valor do parâmetro fim, se o inici não for especificado o valor padrão sera 0, e caso o fim não seja definido sera especificado o valor padrão de 1





