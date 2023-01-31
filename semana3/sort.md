<p align="right">
   <a href="https://patyfil.github.io/cs50-cc50-harvard/">Voltar ao README</a>
</p>
<p align="right">
   <a href="https://patyfil.github.io/cs50-cc50-harvard/3-Algoritmos.html">Voltar ao Índice da Semana 3</a>
</p>

# [Laboratório 3 - Sort (Ordenar)](https://cs50.harvard.edu/x/2023/labs/3/)  

Analise três programas de classificação para determinar quais algoritmos eles usam.  

Obs: Caso ocorra o erro: **Permission denied**  

<img src="../assets/aula3/erroPermissionDeniedSolution.jpg" />  

A solução é dar permissão para o usuário digitando:  

`chmod 700 sort(nr)`

# Começando  

Abra o [VS Code](https://code.cs50.io/)

1 - Entre no *Terminal* do VsCode: `Ctrl`+`'`  

2 - Entrar nessa pasta: `cd pset3`  
OBS: Caso a pasta possua espaço, por exemplo: *Semana 3*  
Será necessário colocar aspas para entrar na pasta: `cd 'Semana 3'` 

3 - No terminal digite o comando: `wget https://cdn.cs50.net/2022/fall/labs/3/sort.zip`  
seguido de *ENTER* para baixar o arquivo zipado [sort.zip](../assets/ArquivosZips/semana3/sort.zip) que contem a pasta *sort* com seus arquivos.  

4 - Execute o unzip: `unzip sort.zip` para extrair a pasta *sort* dentro da pasta *pset3*.  

5 - Você não precisa mais do arquivo ZIP, então você pode executar o comando para excluir: `rm sort.zip`  

6 - Agora entre na pasta: `cd sort`  

7 - Se tudo foi bem sucedido, você deve executar o comando `ls` que listará os arquivos dentro dessa pasta, nesse caso deverá ter uma coleção de `.txt` arquivos ao lado de programas executáveis `sort1`, `sort2` `sort3`.  

Se você tiver algum problema, siga estas mesmas etapas novamente e veja se consegue determinar onde errou!

8 - Leia as instruções logo abaixo;

9 - Teste seu código: `check50 cs50/labs/2023/x/sort`;  

10 - Envie seu código: `submit50 cs50/labs/2023/x/sort` depois digite: `yes`  

&nbsp;

[Ver o progresso no Curso](https://cs50.me/cs50x)

&nbsp;

# Detalhes de Implementação

Lembre-se da aula em que vimos alguns algoritmos para classificar uma sequência de números. Eram eles: selection sort, bubble sort e merge sort.

A `selection` sort itera através das partes não classificadas de uma lista, selecionando o menor elemento a cada vez e movendo-o para seu local. correto.  
Order of n² (Cenário de pior caso - matriz não classificada)  
Omega n²    (Cenário de Melhor Caso - Matriz Ordenada)  
Theta n²

A `bubble sort` compara pares de valores adjacentes, um de cada vez, e os troca se estiverem na ordem incorreta. Isso continua até que a lista seja classificada.  
Order of n² (Cenário de pior caso - matriz não classificada)  
Omega n     (Cenário de Melhor Caso - Matriz Ordenada)  

A `merge sort` divide recursivamente a lista em duas repetidamente e, em seguida, mescla as listas menores de volta em uma maior na ordem correta. 
Order of (n log n) (Cenário de pior caso - matriz não classificada)  
Omega (n log n)    (Cenário de Melhor Caso - Matriz Ordenada)  
Theta (n log n)

# Instruções

São fornecidos a você três programas C já compilados, `sort1`, `sort2` e `sort3`. Cada um desses programas implementa um algoritmo de classificação diferente:  

`selection sort` (classificação por seleção),  
`bubble sort` (classificação por bolha) ou  
`merge sort` (classificação por mesclagem).  

(embora não necessariamente nessa ordem!)

Sua tarefa é determinar qual algoritmo de classificação é usado por cada arquivo.  

* `sort1`, `sort2` e `sort3` são arquivos binários, então você não poderá visualizar o código-fonte C de cada um. Para avaliar qual classificação implementa qual algoritmo, execute as classificações em diferentes listas de valores.  
* Vários arquivos `.txt` são fornecidos a você. Esses arquivos contêm `n` linhas de valores, invertidos, embaralhados ou classificados.  
   * Por exemplo, `reversed10000.txt` contém 10.000 linhas de números invertidos de `10000`, enquanto `random10000.txt` contém 10.000 linhas de números que estão em ordem aleatória.  
* Para executar as classificações nos arquivos de texto, no terminal, execute `./[program_name] [text_file.txt]`. Certifique-se de ter usado `cd` para mover para o `sort` diretório!  
   * Por exemplo, para classificar `reversed10000.txt` com `sort1`, execute `./sort1 reversed10000.txt`.  
* Você pode achar útil cronometrar suas classificações. Para fazer isso, execute `time ./[sort_file] [text_file.txt]`.  
   * Por exemplo, você pode executar `time ./sort1 reversed10000.txt` para executar `sort1` em 10.000 números invertidos. No final da saída do seu terminal, você pode olhar o tempo `real` para ver quanto tempo realmente passou durante a execução do programa.  
* Registre suas respostas em `answers.txt`, juntamente com uma explicação para cada programa, preenchendo os espaços em branco marcados com `TODO`.  

## DICA  
Os diferentes tipos de arquivos `.txt` podem ajudá-lo a determinar qual classificação é qual. Considere como cada algoritmo funciona com uma lista já classificada. Que tal uma lista invertida? Ou lista embaralhada? Pode ser útil trabalhar em uma lista menor de cada tipo e percorrer cada processo de classificação.  

# DICA - Passo a passo  

Este vídeo irá te ajudar a entender o problema ;)  
Atenção: para adicionar legendas ao vídeo clique no botão CC localizado no Player e selecione a opção "Português (Brasil)".  
Uma excelente aula para você!  
## <img src="../assets/youtube.svg" width=20 /> [Sort - Walkthrough - CS50 Labs 2020](https://youtu.be/-Bhxxw6JKKY)

## <img src="../assets/youtube.svg" width=20 /> [CC50: Lab 3 - Sort (Fundação Estudar)](https://youtu.be/I0czI4NM710)

&nbsp;

# Não sabe como resolver?  

## <img src="../assets/youtube.svg" width=20 /> [Sort - Solution - CS50 Labs 2020](https://youtu.be/uOYhrBs37j0)

&nbsp;

<p align="right">
   <a href="https://patyfil.github.io/cs50-cc50-harvard/">Voltar ao README</a>
</p>
<p align="right">
   <a href="https://patyfil.github.io/cs50-cc50-harvard/3-Algoritmos.html">Voltar ao Índice da Semana 3</a>
</p>