# Caixa-Eletronico //name

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>
int main()
{
char saque=0,saldo=0,deposito=0,operacao,sair;
do
{
printf("\n<a>Consultar Saldo\n<b>Deposito\n<c> Saque\n<d>Sair\n");
scanf("%c",&operacao);
system("PAUSE");
switch(operacao)
{
case 'a':
saldo=-saque+deposito;deposito;
printf("Saldo......R$%d\n",saldo);
system("PAUSE");
break;
case 'b':
printf(" Digite o Valor a Ser Depositado:R$");
scanf("%d",&deposito);
saldo=(deposito)+(saldo);
printf("Seu saldo eh:R$ %d\n",saldo);
system("PAUSE");
break;
case 'c':
printf("Digite o Valor Solicitado:R$");
scanf("%d",&saque);
system("PAUSE");
if (saque>saldo)
{
printf("Valor Solicitado R$%d eh menor que o saldo disponivel que eh R$%d\n",saque,saldo);
saque=(0);
system("PAUSE");
}
else if (saque<=saldo)
{
saldo=(deposito)-saque;
printf("Seu novo Saldo eh:R$%d",&saldo);
}
break;
case 'd':
printf("Obrigado por Utilizar nosso serviço ");
getch();
return(0);
}
}while(true);
return 0;
}
