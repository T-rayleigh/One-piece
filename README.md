#include<stdio.h>
#include<string.h>
int main(){
	float AV1,AV2,media;
	char situacao [20];
	printf("Digite anota da AV1 do aluno: ");
	scanf("%f",&AV1);
	printf("Digite a nota da AV2 do aluno: ");
	scanf("%f",&AV2);
	media=(AV1+AV2)/2;
	if(media>=6){
		strcpy(situacao,"aprovado");
	}else{
		strcpy(situacao,"reprovado");
		
	}
	//Exibicao em formato de tabela
	printf("\n===================================\n");
	printf("BOLETIM DO ALUNO\n");
	printf("=====================================\n");
	printf("|AV1 |AV2 2 |MEDIA|SITUACAO|\n");
	printf("---------------------\n");
	printf("|%-5.2f|%-5.2f|%6.2f|%-9s|\n",AV1,AV2,media,situacao);
	printf("==================================\n");
	return 0;
	
}
