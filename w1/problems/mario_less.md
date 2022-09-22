

//MATRÍCULA: 20212045050282
//NOME: Paulo Afonso Pamplona de Carvalho Junior
//USUÁRIO: Junior-jrp



#include <cs50.h>
#include <stdio.h>

int main(void)
{
    int altura;

    //Pedir ao usuario a altura 
    do
    {
    altura = get_int("Altura: \n");
    }

     // garantir que o usuario escolhaa entre  1 e 8
    while 
    ((altura < 1) || (altura > 8)); 

    // for loop para criar a altura da linha
    for (int linha = 0; linha < altura; linha++)
    {
        // for loop cria a largura da pirâmide
        for (int coluna = 0; coluna < altura; coluna++)
        {
            // se a linha mais a coluna for maior ou igual à altura -1 espaço imprime os hashes
            if (linha + coluna >= altura - 1) 
                printf("#");

            // adicionando espaços
            else 
            printf(" ");
        }
        printf("\n");
    }
}
