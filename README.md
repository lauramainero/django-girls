## POO
### 
```python
class Animal:
    def __init__(self, racional, pernas):
        self.racional = racional
        self.pernas = pernas

    def faz_som(self):
        print("barulho")

class Cachorro(Animal):
    def __init__(self, racional, pernas, amizade):
        super().__init__(racional, pernas)
        self.amizade = amizade
    
    def faz_som(self):
        print("auau")
    
animal1 = Cachorro(False, 4, True)
animal1.faz_som()

class Conta:
    def __init__(self, saldo, cpf):
        self.__saldo = saldo
        self.cpf = cpf

    def get_saldo(self):
        return self.__saldo
    def set_saldo(self, saldo):
        self.__saldo = saldo

conta = Conta(1000, 12312312322)
print(conta.get_saldo())
conta.set_saldo(2000)
print(conta.get_saldo())
```