# Clientes
# 5 cadastro, para mais basta alterar dentro do for o número de cadastros desejados

class cadastro:
  def __init__(self, nome=None, cpf=None, idade=None):
    self.nome = nome
    self.cpf = cpf
    self.idade = idade

  def cadastrar_cliente(self):
    self.nome = input("Digite o nome do cliente: ")
    self.cpf = input("Digite o CPF do cliente: ")
    self.idade = int(input("Digite a idade do cliente: "))

  def mostrar_clientes(self):
    print(f"Nome: {self.nome}")
    print(f"CPF: {self.cpf}")
    print(f"Idade: {self.idade}")


clientes = []
for i in range(5):
  cliente = cadastro()
  cliente.cadastrar_cliente()
  cliente.mostrar_clientes()
  clientes.append(cliente)

print("------CLIENTES-----")
for cliente in clientes:
  cliente.mostrar_clientes()
