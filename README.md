# Phyton
📘 Sobre este Repositório:
Este repositório foi criado para armazenar meus primeiros códigos em Python 🐍, desenvolvidos durante as aulas de Ciências da Computação no UniCEUB 🎓.

💡 Os códigos aqui são simples e básicos, frutos de experiências práticas em sala de aula — exercícios, estudos e desafios propostos pelos professores.

🗂️ Ao longo da minha jornada acadêmica, vou continuar atualizando este espaço com tudo o que eu for aprendendo na área de programação, algoritmos e desenvolvimento de software 💻.

Sinta-se à vontade para explorar! 🚀


def lista()
    lista = list(range(1, 11))
    print(lista)
def um_por_um():
    for numero in range(1, 11):
        print(numero)

def com_passo():
    for numero in range(5, 50, 5):
        print(numero)

def regressivo():
    for numero in range(100, 0 -2):
        print(numero)


#lista()
um_por_um()
com_passo()
regressivo()
print()


import mysql.connector

cnx = mysql.connector.connect(user='root', password='ceub123456', host='localhost', database='db_teste')
cs = cnx.cursor()
sql = "SELECT * FROM aluno;"
cs.execute(sql, [])

for (ra, nome, nota1, nota2) in cs:
    print(ra, nome, nota1, nota2)
    media = (nota1 + nota2) / 2
    print('Média=', media)
    if media >= 5:
        print('Aprovado')
    else:
        print('Reprovado')
    print('-' * 30)

# Constantes com as cotações de hoje
EURO = 6.3492
DOLAR = 5.81
YUAN = 0.8039

print('*' * 30)
print('Digite o valor em real R$ para converter:')
real = float(input())
print('*' * 30)

em_euro = real / EURO
em_dolar = real / DOLAR
em_yuan = real / YUAN

print(f'R$ {real} são {em_euro:.2f} euros.')
print(f'R$ {real} são {em_dolar} dolares.')
print(f'R$ {real} são {em_yuan} yuan.')


