# 🏦 Conta Bancária - POO Encapsulamento

Um projeto educacional demonstrando os princípios de **Encapsulamento** em Programação Orientada a Objetos (POO) com Python.

## 📝 Descrição

Este projeto implementa uma classe `ContaBancaria` que exemplifica o conceito de encapsulamento, utilizando atributos privados (prefixo `_`) para proteger os dados internos da classe.

## 🎯 Conceitos Abordados

- **Encapsulamento**: Proteção de dados internos através de atributos privados
- **Validação de Dados**: Validação de valores nas operações bancárias
- **Métodos de Acesso**: Métodos para interagir com dados protegidos

## 💻 Como Funciona

### Classe: `ContaBancaria`

#### Atributos:
- `_saldo` (float): Saldo da conta (privado)
- `_titular` (str): Nome do titular da conta (privado)

#### Métodos:

| Método | Descrição | Validação |
|--------|-----------|-----------|
| `depositar(valor)` | Realiza depósito na conta | Valor deve ser positivo |
| `sacar(valor)` | Realiza saque na conta | Valor deve ser positivo e saldo suficiente |
| `exibir_saldo()` | Exibe saldo atual formatado | - |

## 🚀 Uso

```python
# Criar uma conta bancária
conta1 = ContaBancaria(saldo=2000, titular="Rodrigo")

# Realizar depósito
print(conta1.depositar(valor=600))
# Output: Depósito de R$ 600.00 realizado com sucesso.

# Realizar saque
print(conta1.sacar(valor=1500))
# Output: Saque de R$ 1500.00 realizado com sucesso.

# Exibir saldo
print(conta1.exibir_saldo())
# Output: Saldo atual de R$ 1100.00
```

## ✅ Validações Implementadas

- ✔️ Valores de depósito e saque devem ser positivos
- ✔️ Verificação de saldo suficiente antes de sacar
- ✔️ Mensagens de feedback para cada operação

## 🔒 Princípios de Encapsulamento

O uso de atributos privados (`_saldo`, `_titular`) garante que:
- Os dados não sejam modificados diretamente
- Apenas os métodos da classe possam alterar os valores
- A integridade dos dados seja mantida através de validações

## 📦 Requisitos

- Python 3.6+

## 🔧 Executar

```bash
python encaps.py
```

## 📚 Recursos Adicionais

Para aprender mais sobre encapsulamento em Python, consulte:
- [Python OOP Documentation](https://docs.python.org/3/tutorial/classes.html)
- [Encapsulamento em POO](https://www.w3schools.com/python/python_classes.asp)

---

**Autor**: rodrigomonte07  
**Data**: 2026-04-17