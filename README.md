Nesta pasta se encontra a primeira tarefa de Fisica computacional. 

# Algoritmos de Gradiente Descendente

Este projeto contém implementações do algoritmo de **gradiente descendente** para diferentes funções objetivo. O objetivo é visualizar o comportamento do algoritmo com diferentes taxas de aprendizado e configurações iniciais.

---

## 🧮 Exercício 1

Implemente o algoritmo de gradiente descendente para encontrar o mínimo da função:

\[
U(x) = x^2 - 1
\]

- **Taxa de aprendizado**: \(\alpha = 0.1\)  
- **Tolerância**: \(\epsilon = 0.01\)  
- **Máximo de iterações**: 1000  
- **Condição inicial**: \(x_0 = 5\)

📉 **Tarefa**:  
- Ilustre o algoritmo com um gráfico da função \(U(x)\) e a trajetória da partícula.
- Varie os parâmetros \(\alpha\), \(\epsilon\) e \(x_0\) para ver como afetam a convergência.

  **Resultado**:

  ![U(x) = x^2 - 1](img/EX1.PNG)

---

## 🧮 Exercício 2

Repita o exercício 1 para a função:

\[
U(x) = x^2(x - 1)(x + 1)
\]

- **Condição inicial**: \(x_0 = 2\)

📉 **Tarefa**:  
- Ajuste a taxa de aprendizado \(\alpha\) para fazer o algoritmo convergir ora para um mínimo, ora para outro.
- **Reflexão**: O que você conclui sobre a influência de \(\alpha\) na convergência para mínimos diferentes?

  **Resultado**:

  ![U(x) = x^2(x - 1)(x + 1)](img/ex2.PNG)

---

## 🧮 Exercício 3

Agora manipule a função anterior somando uma reta:

\[
U(x) = x^2(x - 1)(x + 1) + \frac{x}{4}
\]

📉 **Tarefa**:  
- Repita o processo do exercício 2.
- **Reflexão**: Como a adição de um termo linear afeta a convergência e a escolha da taxa de aprendizado \(\alpha\)? 

  **Resultado**:

  ![U(x) = x^2(x - 1)(x + 1) + x/4 ](img/ex3.PNG)

---

## 🧮 Exercício 4

Considere agora uma função bidimensional:

\[
U(\vec{r}) = U(x, y) = \sin(x)\cos(y) + \frac{2(xy)^2}{1000}
\]

A função possui **múltiplos mínimos locais**.

📈 **Visualização**:

1. **Gráfico de contorno**:
   - Use `plt.imshow` ou `plt.pcolormesh` para desenhar a função.
   - Sobreponha a trajetória da partícula no gráfico.

2. **Gráfico de convergência**:
   - Plote o valor de \(U(x_n, y_n)\) em cada iteração \(n\) (semelhante a "epochs" em redes neurais).

🔁 **Parâmetros para explorar**:
- Condições iniciais: \((x_0, y_0)\)
- Taxa de aprendizado \(\alpha\)

💬 **Reflexões**:
- O que acontece ao aumentar/diminuir muito \(\alpha\)?
- Você consegue atingir o **mínimo global**?

   **Resultado**:

 ![U(r) = U(x, y) = sin(x)cos(y) + 2(xy)^2 / 1000](img/ex4.PNG)


---

## 📦 Requisitos

- Python 3
- Bibliotecas: `numpy`, `matplotlib`

Instale com:

```bash
pip install numpy matplotlib
