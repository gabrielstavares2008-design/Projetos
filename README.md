#==================================================
#Calculadora de consumo mensal de um eletrodomestico
#Autor: Gabriel Souza Tavares
#==================================================


# Constantes
Valor_do_KWH=0.80 #Valor fixo em R$ do KWH

#Entrada de dados 
nome_do_aparelho = input (" Digite o nome do seu aparelho:")
potencia_watts = float (input ("Digite a potencia do aparelho em Watts:"))
horas_de_uso = float (input ("Quantas horas ele fica ligado por dia ?"))
#Processamento 
consumoMensal = (potencia_watts * horas_de_uso * 30) / 1000
custo_total = consumoMensal * Valor_do_KWH 
# Saida de dados 

print(f"O valor total em R$ do consumo de energia do aparelho é: R$ {custo_total:.2f}")
