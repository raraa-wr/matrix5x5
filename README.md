# matrix5x5
matrix = [
    [1,2,3,4,5],
    [2,1,3,4,5],
    [3,2,1,4,5],
    [4,3,2,1,5],
    [5,4,3,2,1]
]
matrix2 = [
    [10,9,8,7,6],
    [9,6,7,8,10],
    [8,7,6,9,10],
    [7,6,8,9,10],
    [6,7,8,9,10]
]

result = []

for k in range(5):
    baris = []
    for j in range(5):
        total = 0
        for z in range(5):
            total += matrix[k][z] * matrix2[z][j]
        baris.append(total)
    result.append(baris)

for row in result:
    print(row)
