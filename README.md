# Sistema_Banco.py
Crie do zero uma sistema de banco simples utilizando a linguagem PYTHON, Vamos praticar??

**Desafio:** Criar um Sistema Bancário Simples
Objetivo
Criar um programa em Python que simula um sistema bancário com funcionalidades de depósito, saque e visualização de extrato.

Requisitos
Python instalado no computador
Um editor de texto ou IDE (como Visual Studio Code, PyCharm, etc.)

Passos
# Passo 1: Criação do Menu de Opções
Objetivo: Exibir um menu com opções para o usuário.
*Instruções:*
Crie uma variável menu que contém o texto do menu.
Use print(menu) para exibir o menu.
Exemplo de Código:
Python

menu = """
[d] Depositar
[s] Sacar
[e] Extrato
[q] Sair
=> """
print(menu)

# Passo 2: Configuração das Variáveis Iniciais
Objetivo: Definir variáveis para armazenar o saldo, limite de saque, extrato e contador de saques.
*Instruções:*
Crie variáveis saldo, limite, extrato, numero_saques, e LIMITE_SAQUES com valores iniciais.
Exemplo de Código:
Python

saldo = 0
limite = 500
extrato = ""
numero_saques = 0
LIMITE_SAQUES = 3

# Passo 3: Loop Principal do Programa
Objetivo: Criar um loop que permita ao usuário selecionar opções até decidir sair.
*Instruções:*
Use while True para criar um loop infinito.
Dentro do loop, exiba o menu e leia a opção escolhida pelo usuário.
Adicione uma condição para sair do loop se o usuário escolher a opção q.
Exemplo de Código:
Python

while True:
    opcao = input(menu).lower()
    if opcao == "q":
        print("Obrigado por utilizar nosso sistema")
        break
        
# Passo 4: Implementação da Função de Depósito
Objetivo: Permitir que o usuário deposite dinheiro na conta.
*Instruções:*
Peça ao usuário o valor do depósito.
Verifique se o valor é positivo e adicione ao saldo.
Registre a operação no extrato.
Exemplo de Código:
Python

if opcao == "d":
    valor = float(input("Informe o valor do depósito: "))
    if valor > 0:
        saldo += valor
        extrato += f"Depósito: R$ {valor:.2f}\n"
    else:
        print("Operação falhou! O valor informado é inválido.")
        
# Passo 5: Implementação da Função de Saque
Objetivo: Permitir que o usuário saque dinheiro da conta.
*Instruções:*
Peça ao usuário o valor do saque.
Verifique se o valor é positivo, se não excede o saldo, o limite de saque e o número de saques permitidos.
Subtraia o valor do saldo e registre a operação no extrato.
Exemplo de Código:
Python

if opcao == "s":
    valor = float(input("Informe o valor do saque: "))
    if valor > saldo:
        print("Operação falhou! Você não tem saldo suficiente.")
    elif valor > limite:
        print("Operação falhou! O valor do saque excede o limite.")
    elif numero_saques >= LIMITE_SAQUES:
        print("Operação falhou! Número máximo de saques excedido.")
    elif valor > 0:
        saldo -= valor
        extrato += f"Saque: R$ {valor:.2f}\n"
        numero_saques += 1
    else:
        print("Operação falhou! O valor informado é inválido.")
        
# Passo 6: Implementação da Função de Extrato
Objetivo: Exibir o extrato das transações e o saldo atual.
*Instruções:*
Verifique se houve movimentações e exiba o extrato ou uma mensagem padrão.
Exiba o saldo atual formatado.
Exemplo de Código:
Python

if opcao == "e":
    print("\n================ EXTRATO ================")
    print("Não foram realizadas movimentações." if not extrato else extrato)
    print(f"\nSaldo: R$ {saldo:.2f}")
    print("==========================================")
    
# Teste o Programa
Objetivo: Garantir que todas as funcionalidades estão funcionando corretamente.
Instruções:
Execute o programa.
Realize depósitos, saques e exiba o extrato para verificar se tudo está funcionando como esperado.
Faça ajustes se necessário.

# Parabéns!
# Você completou o desafio de criar um sistema bancário simples em Python. Ótimo trabalho!
