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

# Como a ferramenta integra ao ambiente de desenvolvimento
Para integrar ao VS Code, por exemplo, você pode instalar a extensão "Python" e configurar o RUFF como o linter, realizando as seguinte etapa
No arquivo settings.json adicione:

`"python.linting.ruffEnabled": true`

# Tipos de estilos disponibilizados pelo RUFF
PEP 257 

Flake8 

Pylint 

# Regras de estilo
1. E701 – Multiple statements on one line: Esta regra verifica se há múltiplas instruções em uma única linha e pode ser configurada para permitir ou desabilitar.
2. E731 – Do not assign a lambda expression, use a def: Verifica se lambdas são atribuídas a variáveis e sugere a substituição por funções normais (def).
3. F401 – Unused import: Verifica se existem imports que não estão sendo utilizados no código. Isso ajuda a evitar importações desnecessárias.
