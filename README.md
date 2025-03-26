# Procedimentos para utilizar o RUFF no seu código em Python
Primeiramente você deve ter um projeto em python rodando em sua maquina.

# Instalar o Ruff
Abra o terminal e digite o código abaixo.

`pip install ruff`

# Apos baixar no seu projeto você já pode executar
Codigo para formatar uma pasta `ruff format nome_do_arquivo.py`

Codigo para formatar todo o projeto `ruff format`

# Exemplo de aplicação
Temos o *arquivo_funcoes.py* nele contem o seguinte código

```
def soma(a, b): return a + b
def mult(a, b): return a * b
print(soma(5, 10));print(mult(2, 3))
```
Se rodarmos o seguinte código:

`ruff format arquivo_funcoes.py`

Teremos o resultado:

```
def soma(a, b):
    return a + b


def mult(a, b):
    return a * b


print(soma(5, 10))
print(mult(2, 3))
```
