import numpy as np
def c_stochastic(adj_list):
  n = len(adj_list)
  matrix = np.zeros((n, n))
  for col, line in enumerate(adj_list):
    if len(line) > 0:
      for index in line:
        matrix[index][col] = 1/(len(line))
    else:
      for index in range(n):
        matrix[index][col] = 0
  return matrix
  
  iter = 0
max_iter = 6
t = 1
d = 0.85
matriks = np.array(stochastic)

matriks2 = np.array([[d],[d],[d],[d]])

while iter < max_iter:
  print('\nIterasi ', iter)
  hasil = []
  matriks1 = matriks**t
  
  for i in range(len(matriks1)):
    baris = []
    for k in range(len(matriks2[0])):
       val = 0
       for j in range(len(matriks1[i])):
          val += matriks1[i][j] * matriks2[j][k]
       baris.append(val)
    hasil.append(baris)

  print("PR",iter, '=')
  for baris in hasil:
      print(baris)
  iter += 1
  t += 1 
