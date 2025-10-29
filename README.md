[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/ZURhuU0i)
# Calculadora Remota Cliente-Servidor

## Descrição do Sistema

Este sistema implementa uma calculadora remota usando arquitetura cliente-servidor com sockets TCP.

### Funcionalidades

O servidor oferece **4 operações matemáticas**:

1. **sum** - Soma de dois números
2. **sub** - Subtração de dois números  
3. **mul** - Multiplicação de dois números
4. **div** - Divisão de dois números (com proteção contra divisão por zero)

### Arquitetura

- **server.py**: Servidor que escuta na porta 5678, recebe requisições dos clientes, executa as operações e retorna os resultados
- **client.py**: Cliente que se conecta ao servidor, envia operação e operandos, e recebe o resultado
- **constCS.py**: Constantes compartilhadas (HOST e PORT)

### Como Executar

1. Inicie o servidor:
```bash
python server.py
```

2. Em outro terminal, execute o cliente:
```bash
python client.py
```

3. Digite a operação desejada (sum, sub, mul, div) e os dois operandos quando solicitado.