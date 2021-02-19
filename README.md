# Health
# COVID-19 symptom screening 
nome = input('Informe o seu nome: ')
idade = int(input('Informe sua idade: '))
doenca_infectocontagiosa = input('Suspeita de doença infecto-contagiosa? '). upper()

while doenca_infectocontagiosa!='SIM' and doenca_infectocontagiosa!='NÃO':
    print('Resposta inválida. Informe SIM ou NÃO')
    doenca_infectocontagiosacontagiosa = input('Suspeita de doença infecto-contagiosa?').upper()

if doenca_infectocontagiosa=="SIM":
    febre = input('Esteve com febre nos últimos dias?').upper()
    while febre!='SIM' and febre!='NÃO':
        print('Resposta inválida. Informe SIM ou NÃO')
        febre = input('Esteve com febre nos últimos dias?').upper()
    tosse = input('Apresentou tosse ou dificuldade para respirar:').upper()
    while tosse!='SIM' and tosse!='NÃO':
        print('Resposta inválida. Informe SIM ou NÃO')
        tosse = input('Apresentou tosse ou dificuldade para respirar:').upper()
    pessoas_confirmadascovid = input('Esteve em contato próximo com pessoas suspeitas ou confirmadas para Covid-19?').upper()
    while pessoas_confirmadascovid!='SIM' and pessoas_confirmadascovid!='NÃO':
        print('Resposta inválida. Informe SIM ou NÃO')
        pessoas_confirmadascovid = input('Esteve em contato com pessoas suspeitas ou confirmadas para coronavírus?').upper()
    if febre=='SIM' and tosse=='SIM'and pessoas_confirmadascovid=='SIM':
            print('Encaminhe o paciente para sala VERMELHA.')
else:
    print('Encaminhe o paciente para sala VERDE.')

if idade >= 65:
    print('Paciente COM prioridade')
else:
    genero=input('Digite o gênero do paciente: ').upper()
    while genero!='FEMININO' and genero!='MASCULINO':
        print('Digite FEMININO ou MASCULINO')
        genero = input('Digite o gênero do paciente: ').upper()
    if genero=='FEMININO' and idade>10:
        gravidez=input("A paciente está grávida? ").upper()
        while gravidez !='SIM' and gravidez!='NÃO':
            print ('Digite SIM ou NÃO')
            gravidez = input('A paciente está grávida? ').upper()
        if gravidez=='SIM':
            print('Paciente COM prioridade.')
        else:
            print('Paciente SEM prioridade.')
    else:
        print('Paciente SEM prioridade.')
