# Варіант 2 — створення двовимірного масиву 7x7 за зразком із рисунка

n = 7
matrix = [[0]*n for _ in range(n)]

for i in range(n):
    for j in range(n):
        value = n - i - j
        if value > 0:
            matrix[i][j] = value
        else:
            matrix[i][j] = 0

print("Двовимірний масив 7x7:")
for row in matrix:
    for elem in row:
        print(f"{elem:3}", end="")
    print()
