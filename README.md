# Створення та заповнення масиву 7x7
n = 7
array = [[0 for _ in range(n)] for _ in range(n)]

for i in range(n):
    for j in range(n):
        value = n - 1 - max(i, j)
        array[i][j] = max(value, 0)

# Виведення масиву
for row in array:
    print(' '.join(str(elem) for elem in row))
