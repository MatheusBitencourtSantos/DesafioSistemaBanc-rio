# Desafio: Criando um sistema bancário

## Objetivo geral - V1
criar um sistema bancário com as operações: sacar, depositar e visualizar extrato.

## Desafio
Fomos contratados por um grande banco para desenvolver o seu novo sistema. Esse banco deseja modernizar suas operações e para isso escolheu a linguagem python. Para a primeira versão do sistema devemos implementar apenas 3 operações: depóstio, saque e extrato.

## Operação de depósito
Deve ser possível depositar valores potivios para a minha conta bancária. A v1 do projeto trabalha apenas com 1 usuário, desa forma não precisamos nos preocupar em identificar qual é o número da agência e conta bancária. Todos os depósitos devem ser armazenados em uma variável e exibidos na operação extrato.

## Operação de saque
O sistema deve permitir realizar 3 saques diários com limite máximo de R$ 500,00 por saque. Caso o usuário não tenha saldo em conta, o sistema deve exibir uma mensagem informando que não será possível sacar o dinheiro por falta de saldo. Todos os saques devem ser armazenados em uma variável e exibidos na operação de extrato.

## Operação de extrato
Essa operação deve listar todos os depósitos e saques realizados na conta. No fim da listagem deve ser exibido o saldo atual da conta. Se o extrato estiver em branco, exibir a mensagem: "Não foram realizadas movimentações."
Os valores devem ser exibidos utilizando o formato R$ XXX.XX, 
exemplo:
1500.45 = R$ 1500.45


## Objetivo geral - V2
Separar as funções existentes de saque, deposito e extrato em funções. criar duas novas funções: cadastrar usuário (cliente) e cadastrar conta bancária.

## Desafio
Precisamos deixar nosso código mais modularizado, para isso vamos criar funções para as operações existentes: sacar, depositar e visualizar extrato. Além disso, para a versão 2 do nosso sistema precisamos criar duas novas funções: criar usuário (cliente do banco) e criar conta corrente (vincular com usuário).

## Separação em funções
Devemos criar funções para todas as operações do sistema. Para exercitar tudo o que aprendemos até agora, cada função vai ter regra na passagem de argumentos. O retorno e forma como serão chamadas, pode ser definida por você da forma que achar melhor.

## Saque
A função saque deve receber os argumentos apenas por nome (keyword only). Sugestão de argumentos: saldo, valor, extrato, limite, numero_saques, limite_saques. Sugestão de retorno: saldo e extrato.

## Depósito
A função depósito deve receber os argumentos apenas por posição (positional only). Sugestão de argumentos: saldo, valor, extrato. Sugestão de retorno: Saldo e extrato.

## Extrato 
A função extrato deve receber os argumentos por posição e nome (positional only e keyword only). Argumentos posicionais: saldo, argumentos nomeados: extrato.

## Novas funções
Precisamos criar duas novas funções: criar usuário e criar conta corrente. Fique a vontade para criar mais funções, exemplo: listar contas. 

## Criar usuário (Cliente)
O programa deve armazenar os usuários em uma lista, um usuário é composto por: nome, data de nascimento, cpf e endereço. O endereço é uma string com formato: logradouro, nro - bairro - cidade/sigla estado. Deve ser armazenado somente os números do CPF. não podemos cadastrar 2 usuários com o mesmo CPF.

## Criar conta corrente
O programa deve armazenar contas em uma lista, uma conta é composta por: agência, númerp da conta e usuário. O número da conta é sequencial, iniciando em 1. O numero da agência é fixo: "0001". O usuário pode ter mais de uma conta, mas uma conta pertence a somente um usuário. 

### Dica
Para vincular um usuário a uma conta, filte a lista de usuários buscando o número do CPF informado para cada usuário da lista.

