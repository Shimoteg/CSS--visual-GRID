Para fixar os conhecimentos em CSS grid 

#app {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(3, 1fr);
    height: 100vh;

    border: 2px solid green;
}

# Container

# A Altura e aplicada como 100vh (100% view height) ja que foi definido o display como GRID ocupando toda a altura visivel do navegador.

* display: grid; 
    - Ira transformar o display para o formato de grid ("grade")

* grid-template
    - E um shortcut para as seguintes propriedades:
        # columns
        # rows
        # areas

*  grid-template-columns: repeat(3, 1fr);
   grid-template-rows: repeat(3, 1fr);

    - As propriedades alteram a forma em colunas e linhas de acordo com o desejado
    - repeat( @numero de vezes, tamanho )

= Representado por 1fr a divisao ocorre por fraçoes

# Itens

grid-colum / grid-row
  -  start
  -  end
- Define o ponto de inicio e fim do item desejado
- E possivel utilizar o shortcut por fracoes ("1/3")

#app>div:nth-child(1) {
    grid-column-start: 1;
    grid-column-end: 4;
}

div:nth-child()
    - Seleciona o membro filho desejado dentro dos ()

