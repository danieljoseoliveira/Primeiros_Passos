# Primeiros_Passos
Python Programming initiation.

valor_hora = int(input('Digite aqui o valor da sua hora: R$'))

hora_mes = int(input('Digite aqui o número de horas trabalhadas no mês: '))

valor_real = valor_hora * hora_mes

salario_bruto = valor_real

if salario_bruto == 900:

    fgts = (salario_bruto * 11)/100
    inss = (salario_bruto * 10)/100
    descontos = salario_bruto - inss
    #Isento de imposto
    print(f'Seu salário bruto é de :R$  {valor_hora * hora_mes}')
    print(f'(-) IR (isento)')
    print(f'(-) INSS(10%) :R$   {inss}')
    print(f'FGTS :R%    {fgts}')
    print(f'Salário Líquido :R$ {descontos}')

elif salario_bruto == 1500: #desconto do imposto de renda = 5%
    
    fgts = (salario_bruto * 11)/100
    inss = (salario_bruto * 10)/100
    ir = (salario_bruto * 5)/100
    descontos = salario_bruto - (inss + ir)

    print(f'Seu salário bruto é de :R$  {valor_hora * hora_mes}')
    print(f'(-) IR(5%) :R$  {ir}')
    print(f'(-) INSS(10%) :R$   {inss}')
    print(f'FGTS :R%    {fgts}')
    print(f'Salário Líquido :R$ {descontos}')

elif salario_bruto == 2500: #desconto do imposto de renda = 10%
    
    fgts = (salario_bruto * 11)/100
    inss = (salario_bruto * 10)/100
    ir = (salario_bruto * 10)/100
    descontos = salario_bruto - (inss + ir)

    print(f'Seu salário bruto é de :R$  {valor_hora * hora_mes}')
    print(f'(-) IR(10%) :R$  {ir}')
    print(f'(-) INSS(10%) :R$   {inss}')
    print(f'FGTS :R%    {fgts}')
    print(f'Salário Líquido :R$ {descontos}')

elif salario_bruto > 2500: #desconto do imposto de renda = 20%
    
    fgts = (salario_bruto * 11)/100
    inss = (salario_bruto * 10)/100
    ir = (salario_bruto * 20)/100
    descontos = salario_bruto - (inss + ir)

    print(f'Seu salário bruto é de :R$  {valor_hora * hora_mes}')
    print(f'(-) IR(20%) :R$  {ir}')
    print(f'(-) INSS(10%) :R$   {inss}')
    print(f'FGTS :R%    {fgts}')
    print(f'Salário Líquido :R$ {descontos}')
