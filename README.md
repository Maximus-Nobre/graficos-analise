pip install matplotlib
Requirement already satisfied: matplotlib in /usr/local/lib/python3.12/dist-packages (3.10.0)
Requirement already satisfied: contourpy>=1.0.1 in /usr/local/lib/python3.12/dist-packages (from matplotlib) (1.3.3)
Requirement already satisfied: cycler>=0.10 in /usr/local/lib/python3.12/dist-packages (from matplotlib) (0.12.1)
Requirement already satisfied: fonttools>=4.22.0 in /usr/local/lib/python3.12/dist-packages (from matplotlib) (4.60.1)
Requirement already satisfied: kiwisolver>=1.3.1 in /usr/local/lib/python3.12/dist-packages (from matplotlib) (1.4.9)
Requirement already satisfied: numpy>=1.23 in /usr/local/lib/python3.12/dist-packages (from matplotlib) (2.0.2)
Requirement already satisfied: packaging>=20.0 in /usr/local/lib/python3.12/dist-packages (from matplotlib) (25.0)
Requirement already satisfied: pillow>=8 in /usr/local/lib/python3.12/dist-packages (from matplotlib) (11.3.0)
Requirement already satisfied: pyparsing>=2.3.1 in /usr/local/lib/python3.12/dist-packages (from matplotlib) (3.2.5)
Requirement already satisfied: python-dateutil>=2.7 in /usr/local/lib/python3.12/dist-packages (from matplotlib) (2.9.0.post0)
Requirement already satisfied: six>=1.5 in /usr/local/lib/python3.12/dist-packages (from python-dateutil>=2.7->matplotlib) (1.17.0)

import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5, 6, 7]
y = [100, 95, 110, 105, 120, 115, 130]

plt.plot(x,y)
plt.title("Tendência de Estoque Diário")
plt.xlabel("Semana (Dias)")
plt.ylabel("Estoque (Qnt)")
plt.show()

import matplotlib.pyplot as plt

produtos = ['Teclado', 'Mouse', 'Monitor', 'Webcam']
quantidades = [50, 75, 30, 60]

plt.bar(produtos, quantidades, color=['purple', 'lightcoral', 'skyblue', 'gold'])

plt.title("Comparação de Produtos")
plt.xlabel("Categoria de Produtos")
plt.ylabel("Quantidade do Produtos")


plt.show()

import matplotlib.pyplot as plt

categorias = ['Eletrônicos', 'Vestuário', 'Alimentos']
valores = [15000, 8000, 5000]

plt.figure(figsize=(7, 7))
plt.pie(valores, labels=categorias, autopct='%1.1f%%', startangle=90)
plt.title('Proporção do Valor Total de Estoque por Categoria de Produto')
plt.show()

import matplotlib.pyplot as plt

precos = [50, 120, 300, 80, 20]
estoque = [80, 25, 10, 70, 150]


plt.figure(figsize=(8, 6))
plt.scatter(precos, estoque)
plt.title('Relação entre Preço Unitário e Quantidade em Estoque')
plt.xlabel('Preço Unitário (R$)')
plt.ylabel('Quantidade em Estoque')
plt.grid(True)
plt.show()
