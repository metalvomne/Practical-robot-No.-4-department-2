# Розмір масиву
n = 7

# Створюємо порожній масив 7x7, заповнений нулями
matrix = [[0] * n for _ in range(n)]

# Заповнюємо масив за зразком
for i in range(n):
    for j in range(n):
        # Значення зменшується при віддаленні від верхнього лівого кута
        value = n - max(i, j)
        matrix[i][j] = value if value > 0 else 0

# Виводимо масив у зручному вигляді
for row in matrix:
    print(*row)
