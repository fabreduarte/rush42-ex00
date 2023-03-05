Rush42 Projeto 00

O projeto é composto por 3 arquvios, main incluso.
Um projeto em C basicamente é um confjunto de funções que são conectadas no main. 
Nesse caso precisávamos criar uma função que ao inserir parâmetros formasse um retângulo, a função não deveria quebrar nem ficar num loop.
Cada Grupo deveria adicionar caracteres referentes ao seu projeto são escolhidos com base na primeira letra do nome do líder, sua posição no alfabeto e assim fazer um módulo de 5. Nosso caso foi a letra M e ficamos com o rush03. Characteres são A B e C, eles deveriam ser printados quando a função rodasse.

O arquivo Main chama a função rush, que é a função "principal" do projeto, a funcção rush importa a função ft_putchar.

A putchar basciamente faz o que o nome diz, ela coloca um caractere. É uma função void que não necessita de retorno e coloca um caractere.
A função rush já é um pouco mais complexa. Nós importamos a função ft_putchar nesta, porque ela vai ser necessária para o funcionamento da rush.
A função rush pede dois parâmetros do tipo int, x e y.
São criadas duas variáveis logo em seguida, essas variáveis que vão definir quando e onde A B ou C vão aparecer para formar o retângulo.
Uma variável é iniciada em 1 até chegar no valor do Y que estabelece o número de linhas, ou a "altura" do retângulo, para existir uma linha essa variável precisa ser maior que 1. Então iniciámos um while ( como funciona? Simplesmente enquantos as instruções estarem dentro das determinações ela continua rodando) 
Então enquanto a variável for menor ou igual a Y e o X maior que 0 o while continua rodando. Nessa parte da função nos inciamos a outra variável e em seguida começamos um outro while. Neste while fazemos comparativos das variáveis com os parâmetros para definir onde as letras. Esses comparativos são feitos usando Ifs. 
O if funciona também fazendo comparativos, se ele entra nos parâmetros ela vai seguindo, caso contrário ela vai para um else If, que é se o outro não atende os parâmetros do primeiro vamos para esse, adicionamos mais um else if e por fim o último else. E o que eles fazem, se no primeiro atendem os parâmetros adicionamos o A, no segundo o B e no terceiro C, se não se encaixar em nenhum deles um Espaço vazio é adicionado. Ai é feito um auto incremento da variável associada a X até que o while chegue no seu fim. Ao fim desse while se pula uma linha e faz o auto incremento da variável associada ao Y e retorna ao primeiro while e o processo todo se repete até que os paramêtros atribuídos não são mais atendidos e assim termina o código.


Ai voltamos finalmente ao main. No Main a única função que precisa ser chamada é a rush, porque? Porque a função de inserir charactere já é chamada na função rush então não é necessário ser chamada novamente. 

Na main o que acontece, a função rush é chamada os paramêtros são atribuídos e existe um retorno de 0.
E é assim que o programa Roda.

Depois disso é preciso fazer a compilação do código usando gcc e o exerício pede as seguintes flaghs para a sua compilação -Wall -Wextra -Werror;
