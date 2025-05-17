#include <stdio.h>  

int main() {  
    float renda, total_gastos = 0;      
    float qtd_arroz, preco_arroz, qtd_feijao, preco_feijao, qtd_carne, preco_carne;     
    float qtd_detergente, preco_detergente, qtd_sabao, preco_sabao;    
    float qtd_shampoo, preco_shampoo, qtd_pasta, preco_pasta;  

      
    printf("Digite sua renda mensal (R$): ");  
    scanf("%f", &renda);  

        printf("\n=== ALIMENTOS ===\n");  
    printf("Quantidade de arroz (kg): ");  
    scanf("%f", &qtd_arroz);  
    printf("Preco por kg do arroz (R$): ");  
    scanf("%f", &preco_arroz);  

    printf("Quantidade de feijao (kg): ");  
    scanf("%f", &qtd_feijao);  
    printf("Preco por kg do feijao (R$): ");  
    scanf("%f", &preco_feijao);  

    printf("Quantidade de carne (kg): ");  
    scanf("%f", &qtd_carne);  
    printf("Preco por kg da carne (R$): ");  
    scanf("%f", &preco_carne);  

     
    printf("\n=== LIMPEZA ===\n");  
    printf("Quantidade de detergente (un): ");  
    scanf("%f", &qtd_detergente);  
    printf("Preco do detergente (R$): ");  
    scanf("%f", &preco_detergente);  

    printf("Quantidade de sabao em barra (un): ");  
    scanf("%f", &qtd_sabao);  
    printf("Preco do sabao (R$): ");  
    scanf("%f", &preco_sabao);  

     
    printf("\n=== HIGIENE ===\n");  
    printf("Quantidade de shampoo (un): ");  
    scanf("%f", &qtd_shampoo);  
    printf("Preco do shampoo (R$): ");  
    scanf("%f", &preco_shampoo);  

    printf("Quantidade de pasta de dente (un): ");  
    scanf("%f", &qtd_pasta);  
    printf("Preco da pasta de dente (R$): ");  
    scanf("%f", &preco_pasta);  

    
    total_gastos += qtd_arroz * preco_arroz;  
    total_gastos += qtd_feijao * preco_feijao;  
    total_gastos += qtd_carne * preco_carne;  
    total_gastos += qtd_detergente * preco_detergente;  
    total_gastos += qtd_sabao * preco_sabao;  
    total_gastos += qtd_shampoo * preco_shampoo;  
    total_gastos += qtd_pasta * preco_pasta;  

     
    printf("\n=== RESUMO ===\n");  
    printf("Renda mensal: R$ %.2f\n", renda);  
    printf("Total gasto: R$ %.2f\n", total_gastos);  

    if (total_gastos <= renda) {  
        printf("Status: Dentro do orçamento! Saldo: R$ %.2f\n", renda - total_gastos);  
    }  
    else {  
        printf("Status: ALERTA! Gastos excedem a renda em R$ %.2f\n", total_gastos - renda);  
    }  

    return 0;  
}  

