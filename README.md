# Sistema_Banco.py
Crie do zero uma sistema de banco simples utilizando a linguagem PYTHON, Vamos praticar??

**Desafio:** Criar um Sistema Bancário Simples
Objetivo
Criar um programa em Python que simula um sistema bancário com funcionalidades de depósito, saque e visualização de extrato.

Requisitos
Python instalado no computador
Um editor de texto ou IDE (como Visual Studio Code, PyCharm, etc.)

Passos
# Passo 1: Criação do Menu de Opções #
Objetivo: Exibir um menu com opções para o usuário.

*Instruções:*

Crie uma variável menu que contém o texto do menu.
Use print(menu) para exibir o menu.
Exemplo de Código:
Python

![image](https://github.com/Paulo23k/Sistema_Banco.py---PASSO-A-PASSO/assets/143550827/44f2188b-7ef2-402b-8404-a867bcaf4341)



# Passo 2: Configuração das Variáveis Iniciais #
Objetivo: Definir variáveis para armazenar o saldo, limite de saque, extrato e contador de saques.

*Instruções:*

Crie variáveis saldo, limite, extrato, numero_saques, e LIMITE_SAQUES com valores iniciais.
Exemplo de Código:
Python

![image](https://github.com/Paulo23k/Sistema_Banco.py---PASSO-A-PASSO/assets/143550827/145ec439-f48b-4163-9901-8316dce6a2b8)


# Passo 3: Loop Principal do Programa #
Objetivo: Criar um loop que permita ao usuário selecionar opções até decidir sair.

*Instruções:*

Use while True para criar um loop infinito.
Dentro do loop, exiba o menu e leia a opção escolhida pelo usuário.
Adicione uma condição para sair do loop se o usuário escolher a opção q.
Exemplo de Código:
Python

![image](https://github.com/Paulo23k/Sistema_Banco.py---PASSO-A-PASSO/assets/143550827/99098b92-65b9-4992-8fc3-f197835c4bd4)

        
# Passo 4: Implementação da Função de Depósito #
Objetivo: Permitir que o usuário deposite dinheiro na conta.

*Instruções:*

Peça ao usuário o valor do depósito.
Verifique se o valor é positivo e adicione ao saldo.
Registre a operação no extrato.
Exemplo de Código:
Python

![image](https://github.com/Paulo23k/Sistema_Banco.py---PASSO-A-PASSO/assets/143550827/7e16a247-81e5-44fd-a48c-cfb50fd4c0f6)

        
# Passo 5: Implementação da Função de Saque #
Objetivo: Permitir que o usuário saque dinheiro da conta.

*Instruções:*

Peça ao usuário o valor do saque.
Verifique se o valor é positivo, se não excede o saldo, o limite de saque e o número de saques permitidos.
Subtraia o valor do saldo e registre a operação no extrato.
Exemplo de Código:
Python

![image](https://github.com/Paulo23k/Sistema_Banco.py---PASSO-A-PASSO/assets/143550827/d0c73472-adb9-4d48-abec-5fc90ab05ff8)

        
# Passo 6: Implementação da Função de Extrato #
Objetivo: Exibir o extrato das transações e o saldo atual.

*Instruções:*

Verifique se houve movimentações e exiba o extrato ou uma mensagem padrão.
Exiba o saldo atual formatado.
Exemplo de Código:
Python

![image](https://github.com/Paulo23k/Sistema_Banco.py---PASSO-A-PASSO/assets/143550827/855bbed9-fe8e-4f99-a8b1-58b6ee0e55f1)

    
# Teste o Programa #
Objetivo: Garantir que todas as funcionalidades estão funcionando corretamente.

*Instruções:*

Execute o programa.
Realize depósitos, saques e exiba o extrato para verificar se tudo está funcionando como esperado.
Faça ajustes se necessário.

# Parabéns!
# Você completou o desafio de criar um sistema bancário simples em Python. Ótimo trabalho!
