### Solicitar informações do usuário:
```python
quantidade_rodas = int(input("Digite a quantidade de rodas do veículo: "))
peso_bruto = float(input("Digite o peso bruto do veículo em quilogramas: "))
quantidade_pessoas = int(input("Digite a quantidade de pessoas no veículo: "))
```

### Determinar a categoria de habilitação:
```python
if quantidade_rodas == 2 or quantidade_rodas == 3:
    categoria = "A"
elif quantidade_rodas == 4 and quantidade_pessoas <= 8 and peso_bruto <= 3500:
    categoria = "B"
elif quantidade_rodas >= 4 and peso_bruto > 3500 and peso_bruto <= 6000:
    categoria = "C"
elif quantidade_rodas >= 4 and quantidade_pessoas > 8:
    categoria = "D"
elif quantidade_rodas >= 4 and peso_bruto > 6000:
    categoria = "E"
else:
    categoria = "Categoria não determinada"
```

### Exibir a categoria de habilitação:
```python
print(f"A categoria de habilitação necessária para este veículo é: {categoria}")
```
