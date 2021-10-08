# Corretor ortográfico feito no curso Aplicando Técnicas NLP da Alura

Spell Checker feito totalmente em Python.

## Funções
### 1. Inserção de letras
Insere letras faltantes em uma string fatiada. <br>
Exemplo: exeplo -> exemplo<br>
  lado_esquerdo + "m" + lado_direito

### 2. Remoção de letras
Remove letras a mais em uma string fatiada.<br>
Exemplo: exemmplo -> exemplo<br>
  lado_esquerdo + lado_direito[1:]

### 3. Troca de letras
Altera até uma letra trocada de uma string fatiada.<br>
Exemplo: exenplo -> exemplo<br>
  lado_esquerdo + "m" + lado_direito[1:]
  
### 4. Inversão de letras
Altera a ordem das letras de uma string fatiada.<br>
Exemplo: exepmlo -> exemplo<br>
  lado_esquerdo + lado_direito[1] + lado_direito[0] + lado_direito[2:]

Todas funções se aplicam à diferenças de até um caracter de "distância" do correto.<br>

### 5. Probabilidade
Para o corretor analisar todas possibilidades de palavras, é usado um cálculo de probabilidade, usando a quantidade de vezes que cada uma das palavras, geradas pelo corretor, aparecem na lista de vocabulário, assim, retornando a com maior probabilidade.

## Corretor "turbinado"
Ao final do curso, é criado um corretor que repete as operações feitas pelo original, podendo alterar até dois caracteres de distância, porém, a taxa de acerto do "turbinado" acaba sendo menor do que a do original, já que ele pode alterar muito a palavra errada, transformando em outra, com maior probabilidade.
