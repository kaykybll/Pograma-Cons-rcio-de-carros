# Pograma-Cons-rcio-de-carros
#Projeto Consórcio de carro
'''

Salário do comprador (a)
valor do consórcio desejado
valor da prestação sobre anos

Para que o consórcio seja aceito o salario da Pessoa tem que ser 20 % maio
que seu salario, caso contrario o mesmo não ira conseguir o consorcio desjado

'''

salario   = int(input('DIgite seu salário:'))
consorcio = int(input('Digite o valor do consórcio desejado'))
anos      = int(input('em quantos anos deseja pagar:'))


qant_pres = anos * 12
prestação = consorcio / qant_pres
porcento  = salario *20/100


if porcento  > prestação:
    print('seu consórcio foi aprovado !')
    print(' seram {} prestações de R${:.2f} reais'.format(qant_pres, prestação))
else:
    print(' Infelizmente seu consórcio não foi aprovado !')
