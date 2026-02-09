class ContaBancaria():
    def __init__(self, saldo:float, titular:str):
        self._saldo = saldo
        self._titular = titular

    def depositar(self,valor:float):
        if valor <= 0 :
            return "O valor deve ser positivo."
        self._saldo += valor
        return f"Depósito de R$ {valor:.2f} realizado com sucesso."
    
    def sacar(self,valor:float):
        if valor <= 0 :
            return "O valor deve ser positivo."
        if valor <= self._saldo:
            self._saldo -= valor  
            return f"Saque de R$ {valor:.2f} realizado com sucesso."
        else:
            return "Saldo insuficiente."
        
    def exibir_saldo(self):
        return f"Saldo atual de R$ {self._saldo:.2f}"
    
conta1 = ContaBancaria(saldo=2000, titular="Rodrigo")

print(conta1.depositar(valor=600))
print(conta1.sacar(valor=1500))
print(conta1.exibir_saldo())
