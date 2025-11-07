git init
git add .
git commit -m "Adicionando gráficos"
git branch -M main
git remote add origin https://github.com/seu-usuario/graficos-analise.git
git push -u origin main


pip install matplotlib

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
