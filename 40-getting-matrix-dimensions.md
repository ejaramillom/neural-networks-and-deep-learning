# 40 matrix dimensions

- doing forward propagation we know that the

```
lets say we have a network with 5 layers and the folwlowing distribution:

           n(2, 1)
           n(2, 2) n(3, 1)
   n(1, 1) n(2, 3) n(3, 2) 
x1 n(1, 2) n(2, 4) n(3, 3) n(4, 1)
x2 n(1, 3) n(2, 5) n(3, 4) n(4, 2) n(5, 1) y^

n[0] = n[x] = 2 => (x1, x2)

z[1] = vector of activations (3 , 1) or (n[1], 1) vector
x = input features or n[0] vector (the first column) (n[1], 1) vector
w[1] = weights matrix => (n[1], n[0]) matrix

so the weight matrix for the first hidden layer is computed as follows

activations vector (3, 1) = weight matrix (3, 2) * input features vector (2, 1)

```

## general rule for dimensions

- the dimension of the weights matrix `l` and the constan b vector should be

```
w[l] = (n[l], n[l-1])
b[l] = (n[l], 1)
dw[l] = w[l]
db[l] = n[l]
```

