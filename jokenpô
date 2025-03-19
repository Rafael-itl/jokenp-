#include <stdio.h>
#include <string.h>

// Estrutura para armazenar as cartas de países
typedef struct {
    char nome[50];
    int populacao;
    float area;
    float pib;
    int pontos_turisticos;
    float densidade_demografica;
} Carta;

// Função para comparar as cartas de acordo com o atributo escolhido
void comparar_cartas(Carta carta1, Carta carta2, int atributo) {
    switch (atributo) {
        case 1:  // Comparação pelo Nome do País
            printf("\nComparando pelos nomes dos países...\n");
            printf("País 1: %s\n", carta1.nome);
            printf("País 2: %s\n", carta2.nome);
            printf("Empate! O nome dos países não é comparável diretamente.\n");
            break;
        
        case 2:  // Comparação pela População
            printf("\nComparando pela população...\n");
            printf("País 1 (%s): %d habitantes\n", carta1.nome, carta1.populacao);
            printf("País 2 (%s): %d habitantes\n", carta2.nome, carta2.populacao);
            if (carta1.populacao > carta2.populacao) {
                printf("O país %s venceu!\n", carta1.nome);
            } else if (carta1.populacao < carta2.populacao) {
                printf("O país %s venceu!\n", carta2.nome);
            } else {
                printf("Empate!\n");
            }
            break;
        
        case 3:  // Comparação pela Área
            printf("\nComparando pela área...\n");
            printf("País 1 (%s): %.2f km²\n", carta1.nome, carta1.area);
            printf("País 2 (%s): %.2f km²\n", carta2.nome, carta2.area);
            if (carta1.area > carta2.area) {
                printf("O país %s venceu!\n", carta1.nome);
            } else if (carta1.area < carta2.area) {
                printf("O país %s venceu!\n", carta2.nome);
            } else {
                printf("Empate!\n");
            }
            break;
        
        case 4:  // Comparação pelo PIB
            printf("\nComparando pelo PIB...\n");
            printf("País 1 (%s): R$ %.2f\n", carta1.nome, carta1.pib);
            printf("País 2 (%s): R$ %.2f\n", carta2.nome, carta2.pib);
            if (carta1.pib > carta2.pib) {
                printf("O país %s venceu!\n", carta1.nome);
            } else if (carta1.pib < carta2.pib) {
                printf("O país %s venceu!\n", carta2.nome);
            } else {
                printf("Empate!\n");
            }
            break;
        
        case 5:  // Comparação pelos Pontos Turísticos
            printf("\nComparando pelos pontos turísticos...\n");
            printf("País 1 (%s): %d pontos turísticos\n", carta1.nome, carta1.pontos_turisticos);
            printf("País 2 (%s): %d pontos turísticos\n", carta2.nome, carta2.pontos_turisticos);
            if (carta1.pontos_turisticos > carta2.pontos_turisticos) {
                printf("O país %s venceu!\n", carta1.nome);
            } else if (carta1.pontos_turisticos < carta2.pontos_turisticos) {
                printf("O país %s venceu!\n", carta2.nome);
            } else {
                printf("Empate!\n");
            }
            break;
        
        case 6:  // Comparação pela Densidade Demográfica
            printf("\nComparando pela densidade demográfica...\n");
            printf("País 1 (%s): %.2f pessoas por km²\n", carta1.nome, carta1.densidade_demografica);
            printf("País 2 (%s): %.2f pessoas por km²\n", carta2.nome, carta2.densidade_demografica);
            if (carta1.densidade_demografica < carta2.densidade_demografica) {
                printf("O país %s venceu!\n", carta1.nome);  // Menor densidade vence
            } else if (carta1.densidade_demografica > carta2.densidade_demografica) {
                printf("O país %s venceu!\n", carta2.nome);
            } else {
                printf("Empate!\n");
            }
            break;
        
        default:
            printf("\nOpção inválida! Tente novamente.\n");
    }
}

int main() {
    // Definir algumas cartas de exemplo
    Carta carta1 = {"Brasil", 211000000, 8515767.0, 2200000000.0, 100, 25.0};
    Carta carta2 = {"Canadá", 37590000, 9984670.0, 1800000000.0, 50, 3.0};

    int opcao;
    
    // Menu interativo
    do {
        printf("\n=== MENU ===\n");
        printf("1. Nome do País\n");
        printf("2. População\n");
        printf("3. Área\n");
        printf("4. PIB\n");
        printf("5. Pontos Turísticos\n");
        printf("6. Densidade Demográfica\n");
        printf("0. Sair\n");
        printf("Escolha um atributo para comparar (0 a 6): ");
        scanf("%d", &opcao);
        
        if (opcao != 0) {
            comparar_cartas(carta1, carta2, opcao);
        }
    } while (opcao != 0);

    printf("\nFim do programa. Até logo!\n");
    
    return 0;
}
