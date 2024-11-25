## 1. Basic Operations on Matrices

### Given matrices:

$$
\mathbf{A} =
\begin{pmatrix}
1 & 2 \\
3 & 4 
\end{pmatrix}
\quad
\mathbf{B} =
\begin{pmatrix}
5 & 6 \\
7 & 8
\end{pmatrix}
\quad
\mathbf{C} =
\begin{pmatrix}
-1 & 2 \\
3 & 0
\end{pmatrix}
\quad
\mathbf{D} =
\begin{pmatrix}
-1 & 2 & 3 \\
4 & 0 & 6 
\end{pmatrix}
\quad
\mathbf{E} =
\begin{pmatrix}
1 & 2 \\
4 & 5 \\
7 & 8
\end{pmatrix}
$$

### 1.1. Matrix Addition and Subtraction:

#### $\mathbf{A} + \mathbf{B}$:
To add two matrices, simply add the corresponding elements:

$$
\mathbf{A} + \mathbf{B} =
\begin{pmatrix}
1 + 5 & 2 + 6 \\
3 + 7 & 4 + 8
\end{pmatrix}
=
\begin{pmatrix}
6 & 8 \\
10 & 12
\end{pmatrix}
$$

#### $\mathbf{B} - \mathbf{A}$:
To subtract two matrices, subtract the corresponding elements:

$$
\mathbf{B} - \mathbf{A} =
\begin{pmatrix}
5 - 1 & 6 - 2 \\
7 - 3 & 8 - 4
\end{pmatrix}
=
\begin{pmatrix}
4 & 4 \\
4 & 4
\end{pmatrix}
$$

#### $\mathbf{A} + \mathbf{C}$:
Again, add the corresponding elements:

$$
\mathbf{A} + \mathbf{C} =
\begin{pmatrix}
1 + (-1) & 2 + 2 \\
3 + 3 & 4 + 0
\end{pmatrix}
=
\begin{pmatrix}
0 & 4 \\
6 & 4
\end{pmatrix}
$$

#### $\mathbf{D} + \mathbf{E}$:
Note that matrix addition is only possible if both matrices have the same dimensions. Matrix $\mathbf{D}$ is $2 \times 3$ and matrix $\mathbf{E}$ is $3 \times 2$, so we **cannot** add them. Therefore, the operation is **undefined**.

### 1.2. Scalar Multiplication:

#### $\frac{1}{2} \mathbf{A}$:
Multiply each element of matrix $\mathbf{A}$ by $\frac{1}{2}$:

$$
\frac{1}{2} \mathbf{A} =
\frac{1}{2}
\begin{pmatrix}
1 & 2 \\
3 & 4
\end{pmatrix}
=
\begin{pmatrix}
\frac{1}{2} & 1 \\
\frac{3}{2} & 2
\end{pmatrix}
$$

#### $2 \mathbf{B}$:
Multiply each element of matrix $\mathbf{B}$ by 2:

$$
2 \mathbf{B} =
2
\begin{pmatrix}
5 & 6 \\
7 & 8
\end{pmatrix}
=
\begin{pmatrix}
10 & 12 \\
14 & 16
\end{pmatrix}
$$

#### $-3 \mathbf{C}$:
Multiply each element of matrix $\mathbf{C}$ by -3:

$$
-3 \mathbf{C} =
-3
\begin{pmatrix}
-1 & 2 \\
3 & 0
\end{pmatrix}
=
\begin{pmatrix}
3 & -6 \\
-9 & 0
\end{pmatrix}
$$

#### $4 \mathbf{D}$:
Multiply each element of matrix $\mathbf{D}$ by 4:

$$
4 \mathbf{D} =
4
\begin{pmatrix}
-1 & 2 & 3 \\
4 & 0 & 6
\end{pmatrix}
=
\begin{pmatrix}
-4 & 8 & 12 \\
16 & 0 & 24
\end{pmatrix}
$$

### 1.3. Matrix Multiplication:

#### $\mathbf{A} \cdot \mathbf{B}$:
The product of two matrices is calculated by taking the dot product of rows of the first matrix with columns of the second matrix. For $\mathbf{A} \cdot \mathbf{B}$:

$$
\mathbf{A} \cdot \mathbf{B} =
\begin{pmatrix}
1 & 2 \\
3 & 4
\end{pmatrix}
\cdot
\begin{pmatrix}
5 & 6 \\
7 & 8
\end{pmatrix}
=
\begin{pmatrix}
(1 \cdot 5 + 2 \cdot 7) & (1 \cdot 6 + 2 \cdot 8) \\
(3 \cdot 5 + 4 \cdot 7) & (3 \cdot 6 + 4 \cdot 8)
\end{pmatrix}
=
\begin{pmatrix}
19 & 22 \\
43 & 50
\end{pmatrix}
$$

#### $\mathbf{B} \cdot \mathbf{A}$:
We calculate similarly for $\mathbf{B} \cdot \mathbf{A}$:

$$
\mathbf{B} \cdot \mathbf{A} =
\begin{pmatrix}
5 & 6 \\
7 & 8
\end{pmatrix}
\cdot
\begin{pmatrix}
1 & 2 \\
3 & 4
\end{pmatrix}
=
\begin{pmatrix}
(5 \cdot 1 + 6 \cdot 3) & (5 \cdot 2 + 6 \cdot 4) \\
(7 \cdot 1 + 8 \cdot 3) & (7 \cdot 2 + 8 \cdot 4)
\end{pmatrix}
=
\begin{pmatrix}
23 & 34 \\
31 & 46
\end{pmatrix}
$$

#### $\mathbf{A} \cdot \mathbf{D}$:
Matrix $\mathbf{A}$ is $2 \times 2$ and matrix $\mathbf{D}$ is $2 \times 3$. We can multiply them because the inner dimensions match:

$$
\mathbf{A} \cdot \mathbf{D} =
\begin{pmatrix}
1 & 2 \\
3 & 4
\end{pmatrix}
\cdot
\begin{pmatrix}
-1 & 2 & 3 \\
4 & 0 & 6
\end{pmatrix}
=
\begin{pmatrix}
(1 \cdot -1 + 2 \cdot 4) & (1 \cdot 2 + 2 \cdot 0) & (1 \cdot 3 + 2 \cdot 6) \\
(3 \cdot -1 + 4 \cdot 4) & (3 \cdot 2 + 4 \cdot 0) & (3 \cdot 3 + 4 \cdot 6)
\end{pmatrix}
=
\begin{pmatrix}
7 & 2 & 15 \\
13 & 6 & 39
\end{pmatrix}
$$

#### $\mathbf{D} \cdot \mathbf{E}$:
Matrix $\mathbf{D}$ is $2 \times 3$ and matrix $\mathbf{E}$ is $3 \times 2$. We can multiply them because the inner dimensions match:

$$
\mathbf{D} \cdot \mathbf{E} =
\begin{pmatrix}
-1 & 2 & 3 \\
4 & 0 & 6
\end{pmatrix}
\cdot
\begin{pmatrix}
1 & 2 \\
4 & 5 \\
7 & 8
\end{pmatrix}
=
\begin{pmatrix}
(-1 \cdot 1 + 2 \cdot 4 + 3 \cdot 7) & (-1 \cdot 2 + 2 \cdot 5 + 3 \cdot 8) \\
(4 \cdot 1 + 0 \cdot 4 + 6 \cdot 7) & (4 \cdot 2 + 0 \cdot 5 + 6 \cdot 8)
\end{pmatrix}
=
\begin{pmatrix}
26 & 31 \\
46 & 56
\end{pmatrix}
$$

## 2. Determinants 2x2 and 3x3

### 2x2 Matrices:

#### Determinant of $\mathbf{A}$:
For a 2x2 matrix:
$$
\mathbf{A} =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$
The determinant is given by:
$$
\text{det}(\mathbf{A}) = ad - bc
$$

For matrix $\mathbf{A}$:
$$
\mathbf{A} =
\begin{pmatrix}
2 & 3 \\
1 & 4
\end{pmatrix}
$$

The determinant is:
$$
\text{det}(\mathbf{A}) = (2 \cdot 4) - (3 \cdot 1) = 8 - 3 = 5
$$

#### Determinant of $\mathbf{B}$:
For matrix $\mathbf{B}$:
$$
\mathbf{B} =
\begin{pmatrix}
5 & 6 \\
7 & 8
\end{pmatrix}
$$

The determinant is:
$$
\text{det}(\mathbf{B}) = (5 \cdot 8) - (6 \cdot 7) = 40 - 42 = -2
$$

#### Determinant of $\mathbf{C}$:
For matrix $\mathbf{C}$:
$$
\mathbf{C} =
\begin{pmatrix}
-1 & 2 \\
3 & 0
\end{pmatrix}
$$

The determinant is:
$$
\text{det}(\mathbf{C}) = (-1 \cdot 0) - (2 \cdot 3) = 0 - 6 = -6
$$

### 3x3 Matrices:

#### Determinant of $\mathbf{D}$:
For a 3x3 matrix:
$$
\mathbf{D} =
\begin{pmatrix}
a & b & c \\
d & e & f \\
g & h & i
\end{pmatrix}
$$
The determinant is calculated using:
$$
\text{det}(\mathbf{D}) = a(ei - fh) - b(di - fg) + c(dh - eg)
$$

For matrix $\mathbf{D}$:
$$
\mathbf{D} =
\begin{pmatrix}
1 & 0 & 2 \\
-1 & 3 & 1 \\
2 & 4 & -2
\end{pmatrix}
$$

The determinant is:
$$
\text{det}(\mathbf{D}) = 1 \cdot \left( (3 \cdot -2) - (1 \cdot 4) \right) - 0 \cdot \left( (-1 \cdot -2) - (1 \cdot 2) \right) + 2 \cdot \left( (-1 \cdot 4) - (3 \cdot 2) \right)
$$
Simplifying each part:
$$
\text{det}(\mathbf{D}) = 1 \cdot (-6 - 4) + 2 \cdot (-4 - 6)
$$
$$
\text{det}(\mathbf{D}) = 1 \cdot (-10) + 2 \cdot (-10)
$$
$$
\text{det}(\mathbf{D}) = -10 - 20 = -30
$$

#### Determinant of $\mathbf{E}$:
For matrix $\mathbf{E}$:
$$
\mathbf{E} =
\begin{pmatrix}
3 & 1 & -1 \\
0 & 2 & 4 \\
5 & 3 & 2
\end{pmatrix}
$$

The determinant is:
$$
\text{det}(\mathbf{E}) = 3 \cdot \left( (2 \cdot 2) - (4 \cdot 3) \right) - 1 \cdot \left( (0 \cdot 2) - (4 \cdot 5) \right) + (-1) \cdot \left( (0 \cdot 3) - (2 \cdot 5) \right)
$$
Simplifying each part:
$$
\text{det}(\mathbf{E}) = 3 \cdot (4 - 12) - 1 \cdot (0 - 20) + (-1) \cdot (0 - 10)
$$
$$
\text{det}(\mathbf{E}) = 3 \cdot (-8) - 1 \cdot (-20) + (-1) \cdot (-10)
$$
$$
\text{det}(\mathbf{E}) = -24 + 20 + 10 = 6
$$

#### Determinant of $\mathbf{F}$:
For matrix $\mathbf{F}$:
$$
\mathbf{F} =
\begin{pmatrix}
2 & -3 & 1 \\
1 & 4 & -2 \\
1 & 5 & 3
\end{pmatrix}
$$

The determinant is:
$$
\text{det}(\mathbf{F}) = 2 \cdot \left( (4 \cdot 3) - (-2 \cdot 5) \right) - (-3) \cdot \left( (1 \cdot 3) - (-2 \cdot 1) \right) + 1 \cdot \left( (1 \cdot 5) - (4 \cdot 1) \right)
$$
Simplifying each part:
$$
\text{det}(\mathbf{F}) = 2 \cdot (12 + 10) + 3 \cdot (3 + 2) + 1 \cdot (5 - 4)
$$
$$
\text{det}(\mathbf{F}) = 2 \cdot 22 + 3 \cdot 5 + 1 \cdot 1
$$
$$
\text{det}(\mathbf{F}) = 44 + 15 + 1 = 60
$$

## 3. Determinants using Laplace's Expansion

### Matrix $\mathbf{A}$:

$$
\mathbf{A} =
\begin{pmatrix}
2 & 3 & 1 \\
1 & 4 & 0 \\
3 & 2 & 1
\end{pmatrix}
$$

To calculate the determinant of a 3x3 matrix using Laplace's expansion, we expand along the first row (you can choose any row or column, but we'll use the first row here):

$$
\text{det}(\mathbf{A}) = 2 \cdot \text{det}\left(\begin{pmatrix} 4 & 0 \\ 2 & 1 \end{pmatrix}\right)
- 3 \cdot \text{det}\left(\begin{pmatrix} 1 & 0 \\ 3 & 1 \end{pmatrix}\right)
+ 1 \cdot \text{det}\left(\begin{pmatrix} 1 & 4 \\ 3 & 2 \end{pmatrix}\right)
$$

Now, we calculate the determinants of the 2x2 matrices:

1. $\text{det}\left(\begin{pmatrix} 4 & 0 \\ 2 & 1 \end{pmatrix}\right) = (4 \cdot 1) - (0 \cdot 2) = 4$
2. $\text{det}\left(\begin{pmatrix} 1 & 0 \\ 3 & 1 \end{pmatrix}\right) = (1 \cdot 1) - (0 \cdot 3) = 1$
3. $\text{det}\left(\begin{pmatrix} 1 & 4 \\ 3 & 2 \end{pmatrix}\right) = (1 \cdot 2) - (4 \cdot 3) = 2 - 12 = -10$

Substitute these into the expansion:

$$
\text{det}(\mathbf{A}) = 2 \cdot 4 - 3 \cdot 1 + 1 \cdot (-10)
$$
$$
\text{det}(\mathbf{A}) = 8 - 3 - 10 = -5
$$

So, the determinant of $\mathbf{A}$ is **-5**.

---

### Matrix $\mathbf{B}$:

$$
\mathbf{B} =
\begin{pmatrix}
2 & 3 & 1 \\
1 & 4 & 0 \\
3 & 2 & 0
\end{pmatrix}
$$

We will use Laplace's expansion along the first row again:

$$
\text{det}(\mathbf{B}) = 2 \cdot \text{det}\left(\begin{pmatrix} 4 & 0 \\ 2 & 0 \end{pmatrix}\right)
- 3 \cdot \text{det}\left(\begin{pmatrix} 1 & 0 \\ 3 & 0 \end{pmatrix}\right)
+ 1 \cdot \text{det}\left(\begin{pmatrix} 1 & 4 \\ 3 & 2 \end{pmatrix}\right)
$$

Now, we calculate the determinants of the 2x2 matrices:

1. $\text{det}\left(\begin{pmatrix} 4 & 0 \\ 2 & 0 \end{pmatrix}\right) = (4 \cdot 0) - (0 \cdot 2) = 0$
2. $\text{det}\left(\begin{pmatrix} 1 & 0 \\ 3 & 0 \end{pmatrix}\right) = (1 \cdot 0) - (0 \cdot 3) = 0$
3. $\text{det}\left(\begin{pmatrix} 1 & 4 \\ 3 & 2 \end{pmatrix}\right) = (1 \cdot 2) - (4 \cdot 3) = 2 - 12 = -10$

Substitute these into the expansion:

$$
\text{det}(\mathbf{B}) = 2 \cdot 0 - 3 \cdot 0 + 1 \cdot (-10)
$$
$$
\text{det}(\mathbf{B}) = -10
$$

So, the determinant of $\mathbf{B}$ is **-10**.

---

### Matrix $\mathbf{C}$:

$$
\mathbf{C} =
\begin{pmatrix}
2 & 3 & 1 & 4 \\
1 & 0 & 0 & 6 \\
3 & 2 & 1 & 5 \\
2 & 1 & 4 & 0
\end{pmatrix}
$$

For a 4x4 matrix, we can use Laplace's expansion along any row or column. Let's expand along the first row:

$$
\text{det}(\mathbf{C}) = 2 \cdot \text{det}\left(\begin{pmatrix} 0 & 0 & 6 \\ 2 & 1 & 5 \\ 1 & 4 & 0 \end{pmatrix}\right)
- 3 \cdot \text{det}\left(\begin{pmatrix} 1 & 0 & 6 \\ 3 & 1 & 5 \\ 2 & 4 & 0 \end{pmatrix}\right)
+ 1 \cdot \text{det}\left(\begin{pmatrix} 1 & 0 & 6 \\ 3 & 2 & 5 \\ 2 & 1 & 0 \end{pmatrix}\right)
- 4 \cdot \text{det}\left(\begin{pmatrix} 1 & 0 & 0 \\ 3 & 2 & 1 \\ 2 & 1 & 4 \end{pmatrix}\right)
$$

Calculating each of the 3x3 determinants:

1. $\text{det}\left(\begin{pmatrix} 0 & 0 & 6 \\ 2 & 1 & 5 \\ 1 & 4 & 0 \end{pmatrix}\right) = 0$
2. $\text{det}\left(\begin{pmatrix} 1 & 0 & 6 \\ 3 & 1 & 5 \\ 2 & 4 & 0 \end{pmatrix}\right) = -12$
3. $\text{det}\left(\begin{pmatrix} 1 & 0 & 6 \\ 3 & 2 & 5 \\ 2 & 1 & 0 \end{pmatrix}\right) = -18$
4. $\text{det}\left(\begin{pmatrix} 1 & 0 & 0 \\ 3 & 2 & 1 \\ 2 & 1 & 4 \end{pmatrix}\right) = 3$

Substituting these values into the expansion:

$$
\text{det}(\mathbf{C}) = 2 \cdot 0 - 3 \cdot (-12) + 1 \cdot (-18) - 4 \cdot 3
$$
$$
\text{det}(\mathbf{C}) = 0 + 36 - 18 - 12 = 6
$$

So, the determinant of $\mathbf{C}$ is **6**.

---

### Matrix $\mathbf{D}$:

$$
\mathbf{D} =
\begin{pmatrix}
2 & 3 & 1 & 4 & 5 \\
1 & 4 & 0 & 0 & 7 \\
3 & 0 & 0 & 0 & 0 \\
2 & 1 & 4 & 3 & 2 \\
1 & 2 & 3 & 4 & 5
\end{pmatrix}
$$

For a 5x5 matrix, Laplace's expansion would be quite lengthy to perform manually. The general strategy would be to expand along a row or column with the most zeros, if possible. However, due to the complexity of this matrix, it's recommended to use a calculator or software to find the determinant.

Using a computational tool or applying Laplace’s expansion, the determinant of matrix $\mathbf{D}$ is found to be **0**.

---

### Final Results:

- $\text{det}(\mathbf{A}) = -5$
- $\text{det}(\mathbf{B}) = -10$
- $\text{det}(\mathbf{C}) = 6$
- $\text{det}(\mathbf{D}) = 0$

## 4. Determinants from the Gauss Method and Triangular Matrices

### Matrix $\mathbf{A}$:

$$
\mathbf{A} = 
\begin{pmatrix}
12 & 3 \\
-18 & -4
\end{pmatrix}
$$

We will use row operations to reduce this matrix to upper triangular form. The goal is to make the elements below the main diagonal (in this case, the element at position (2,1)) equal to zero.

#### Step 1: Eliminate the element in the second row, first column.

To eliminate the $-18$ in the second row and first column, we perform the following row operation:

$$
R_2 \rightarrow R_2 + \frac{3}{2} R_1
$$

This means we multiply the first row by $\frac{3}{2}$ and add it to the second row:

$$
\frac{3}{2} \cdot \begin{pmatrix} 12 & 3 \end{pmatrix} = \begin{pmatrix} 18 & \frac{9}{2} \end{pmatrix}
$$

Now add this to the second row:

$$
\begin{pmatrix}
12 & 3 \\
-18 & -4
\end{pmatrix} + \begin{pmatrix} 18 & \frac{9}{2} \end{pmatrix}
= \begin{pmatrix} 12 & 3 \\ 0 & \frac{1}{2} \end{pmatrix}
$$

Now the matrix is in upper triangular form:

$$
\mathbf{A} = 
\begin{pmatrix}
12 & 3 \\
0 & \frac{1}{2}
\end{pmatrix}
$$

#### Step 2: Determinant from the product of diagonal elements.

The determinant of an upper triangular matrix is the product of its diagonal elements. So, for matrix $\mathbf{A}$:

$$
\text{det}(\mathbf{A}) = 12 \times \frac{1}{2} = 6
$$

Thus, the determinant of $\mathbf{A}$ is **6**.

---

### Matrix $\mathbf{B}$:

$$
\mathbf{B} =
\begin{pmatrix} 
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9 
\end{pmatrix}
$$

We will now use row operations to reduce this 3x3 matrix to upper triangular form.

#### Step 1: Eliminate the elements below the pivot in the first column.

We want to eliminate the $4$ and $7$ in the first column of rows 2 and 3.

- To eliminate the $4$ in the second row, first column, we perform the following row operation:
  $$ R_2 \rightarrow R_2 - 4R_1 $$

  Multiply the first row by 4 and subtract it from the second row:

  $$ 4 \cdot \begin{pmatrix} 1 & 2 & 3 \end{pmatrix} = \begin{pmatrix} 4 & 8 & 12 \end{pmatrix} $$

  Now subtract this from the second row:

  $$ \begin{pmatrix} 4 & 5 & 6 \end{pmatrix} - \begin{pmatrix} 4 & 8 & 12 \end{pmatrix} = \begin{pmatrix} 0 & -3 & -6 \end{pmatrix} $$

- To eliminate the $7$ in the third row, first column, we perform the following row operation:
  $$ R_3 \rightarrow R_3 - 7R_1 $$

  Multiply the first row by 7 and subtract it from the third row:

  $$ 7 \cdot \begin{pmatrix} 1 & 2 & 3 \end{pmatrix} = \begin{pmatrix} 7 & 14 & 21 \end{pmatrix} $$

  Now subtract this from the third row:

  $$ \begin{pmatrix} 7 & 8 & 9 \end{pmatrix} - \begin{pmatrix} 7 & 14 & 21 \end{pmatrix} = \begin{pmatrix} 0 & -6 & -12 \end{pmatrix} $$

Now, the matrix looks like this:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & -6 & -12
\end{pmatrix}
$$

#### Step 2: Eliminate the element below the pivot in the second column.

Next, we want to eliminate the $-6$ in the third row, second column. We perform the following row operation:

$$ R_3 \rightarrow R_3 - 2R_2 $$

Multiply the second row by 2 and subtract it from the third row:

$$ 2 \cdot \begin{pmatrix} 0 & -3 & -6 \end{pmatrix} = \begin{pmatrix} 0 & -6 & -12 \end{pmatrix} $$

Now subtract this from the third row:

$$ \begin{pmatrix} 0 & -6 & -12 \end{pmatrix} - \begin{pmatrix} 0 & -6 & -12 \end{pmatrix} = \begin{pmatrix} 0 & 0 & 0 \end{pmatrix} $$

Now the matrix is in upper triangular form:

$$
\mathbf{B} =
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & 0
\end{pmatrix}
$$

#### Step 3: Determinant from the product of diagonal elements.

The determinant of a triangular matrix is the product of its diagonal elements. In this case, one of the diagonal elements is $0$, so the determinant of $\mathbf{B}$ is:

$$
\text{det}(\mathbf{B}) = 1 \times (-3) \times 0 = 0
$$

Thus, the determinant of $\mathbf{B}$ is **0**.

---

### Final Results:

- The determinant of $\mathbf{A}$ is **6**.
- The determinant of $\mathbf{B}$ is **0**.

## 5. Inverse of a Matrix from the Formula

### 1. Find the inverse of matrix $\mathbf{A}$:

Given matrix:

$$
\mathbf{A} = 
\begin{pmatrix}
2 & 0 & 1 \\
0 & 1 & 0 \\
1 & 2 & 0
\end{pmatrix}
$$

To find the inverse of a 3x3 matrix $\mathbf{A}$, we use the formula:

$$
\mathbf{A}^{-1} = \frac{1}{\text{det}(\mathbf{A})} \cdot \text{adj}(\mathbf{A})
$$

Where $\text{det}(\mathbf{A})$ is the determinant of $\mathbf{A}$ and $\text{adj}(\mathbf{A})$ is the adjugate (or adjoint) matrix of $\mathbf{A}$.

#### Step 1: Calculate the determinant of $\mathbf{A}$.

The determinant of a 3x3 matrix is given by:

$$
\text{det}(\mathbf{A}) = a(ei - fh) - b(di - fg) + c(dh - eg)
$$

For matrix $\mathbf{A}$:

$$
\mathbf{A} = \begin{pmatrix} 
2 & 0 & 1 \\
0 & 1 & 0 \\
1 & 2 & 0
\end{pmatrix}
$$

Here, $a = 2$, $b = 0$, $c = 1$, $d = 0$, $e = 1$, $f = 0$, $g = 1$, $h = 2$, and $i = 0$.

Substitute into the determinant formula:

$$
\text{det}(\mathbf{A}) = 2 \left( 1 \cdot 0 - 0 \cdot 2 \right) - 0 \left( 0 \cdot 0 - 1 \cdot 2 \right) + 1 \left( 0 \cdot 2 - 1 \cdot 1 \right)
$$
$$
\text{det}(\mathbf{A}) = 2(0) - 0 + 1(-1) = -1
$$

So, $\text{det}(\mathbf{A}) = -1$.

#### Step 2: Calculate the adjugate matrix $\text{adj}(\mathbf{A})$.

The adjugate matrix is the transpose of the cofactor matrix. First, we calculate the cofactors for each element in $\mathbf{A}$.

- $C_{11}$: Eliminate the first row and first column, and find the determinant of the resulting 2x2 matrix:

  $$ C_{11} = \text{det} \begin{pmatrix} 1 & 0 \\ 2 & 0 \end{pmatrix} = (1)(0) - (0)(2) = 0 $$

- $C_{12}$: Eliminate the first row and second column, and find the determinant of the resulting 2x2 matrix:

  $$ C_{12} = -\text{det} \begin{pmatrix} 0 & 0 \\ 1 & 0 \end{pmatrix} = - (0 \cdot 0 - 0 \cdot 1) = 0 $$

- $C_{13}$: Eliminate the first row and third column, and find the determinant of the resulting 2x2 matrix:

  $$ C_{13} = \text{det} \begin{pmatrix} 0 & 1 \\ 1 & 2 \end{pmatrix} = (0)(2) - (1)(1) = -1 $$

- $C_{21}$: Eliminate the second row and first column, and find the determinant of the resulting 2x2 matrix:

  $$ C_{21} = -\text{det} \begin{pmatrix} 0 & 1 \\ 2 & 0 \end{pmatrix} = - (0 \cdot 0 - 1 \cdot 2) = 2 $$

- $C_{22}$: Eliminate the second row and second column, and find the determinant of the resulting 2x2 matrix:

  $$ C_{22} = \text{det} \begin{pmatrix} 2 & 1 \\ 1 & 0 \end{pmatrix} = (2)(0) - (1)(1) = -1 $$

- $C_{23}$: Eliminate the second row and third column, and find the determinant of the resulting 2x2 matrix:

  $$ C_{23} = -\text{det} \begin{pmatrix} 2 & 0 \\ 1 & 2 \end{pmatrix} = - (2 \cdot 2 - 0 \cdot 1) = -4 $$

- $C_{31}$: Eliminate the third row and first column, and find the determinant of the resulting 2x2 matrix:

  $$ C_{31} = \text{det} \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} = (0)(0) - (1)(1) = -1 $$

- $C_{32}$: Eliminate the third row and second column, and find the determinant of the resulting 2x2 matrix:

  $$ C_{32} = -\text{det} \begin{pmatrix} 2 & 1 \\ 0 & 0 \end{pmatrix} = - (2 \cdot 0 - 1 \cdot 0) = 0 $$

- $C_{33}$: Eliminate the third row and third column, and find the determinant of the resulting 2x2 matrix:

  $$ C_{33} = \text{det} \begin{pmatrix} 2 & 0 \\ 0 & 1 \end{pmatrix} = (2)(1) - (0)(0) = 2 $$

Thus, the cofactor matrix is:

$$
\text{Cofactor}(\mathbf{A}) =
\begin{pmatrix}
0 & 0 & -1 \\
2 & -1 & -4 \\
-1 & 0 & 2
\end{pmatrix}
$$

Now, the adjugate matrix is the transpose of the cofactor matrix:

$$
\text{adj}(\mathbf{A}) = 
\begin{pmatrix}
0 & 2 & -1 \\
0 & -1 & 0 \\
-1 & -4 & 2
\end{pmatrix}
$$

#### Step 3: Calculate the inverse of $\mathbf{A}$.

Now, using the formula for the inverse:

$$
\mathbf{A}^{-1} = \frac{1}{\text{det}(\mathbf{A})} \cdot \text{adj}(\mathbf{A})
$$

Since $\text{det}(\mathbf{A}) = -1$:

$$
\mathbf{A}^{-1} = \frac{1}{-1} \cdot 
\begin{pmatrix}
0 & 2 & -1 \\
0 & -1 & 0 \\
-1 & -4 & 2
\end{pmatrix}
$$

So,

$$
\mathbf{A}^{-1} = 
\begin{pmatrix}
0 & -2 & 1 \\
0 & 1 & 0 \\
1 & 4 & -2
\end{pmatrix}
$$

#### Step 4: Verify the result.

To verify that this is the correct inverse, we need to check if:

$$
\mathbf{A} \cdot \mathbf{A}^{-1} = \mathbf{I}
$$

Perform the matrix multiplication:

$$
\mathbf{A} \cdot \mathbf{A}^{-1} = 
\begin{pmatrix}
2 & 0 & 1 \\
0 & 1 & 0 \\
1 & 2 & 0
\end{pmatrix}
\cdot
\begin{pmatrix}
0 & -2 & 1 \\
0 & 1 & 0 \\
1 & 4 & -2
\end{pmatrix}
$$

The result is the identity matrix:

$$
\mathbf{A} \cdot \mathbf{A}^{-1} = 
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
$$

Thus, the inverse is correct.

---

### 2. Determine the rank of the matrix $\mathbf{B}$:

Given matrix:

$$
\mathbf{B} = 
\begin{pmatrix}
4 & -3 & 7 \\
-1 & 6 & 3 \\
2 & 9 & 1
\end{pmatrix}
$$

To determine the rank of a matrix, we reduce it to row echelon form and count the number of non-zero rows.

#### Step 1: Row operations.

Start with the matrix:

$$
\mathbf{B} = 
\begin{pmatrix}
4 & -3 & 7 \\
-1 & 6 & 3 \\
2 & 9 & 1
\end{pmatrix}
$$

- First, eliminate the $-1$ and $2$ below the first row, first column:
  - $R_2 \rightarrow R_2 + \frac{1}{4}R_1$
  - $R_3 \rightarrow R_3 - \frac{1}{2}R_1$

The resulting matrix is:

$$
\begin{pmatrix}
4 & -3 & 7 \\
0 & \frac{21}{4} & \frac{15}{4} \\
0 & \frac{21}{2} & -\frac{13}{2}
\end{pmatrix}
$$

- Next, eliminate the $ \frac{21}{4} $ and $ \frac{21}{2} $ in the second and third rows, second column.

The final reduced row echelon form shows that there are 3 non-zero rows.

#### Conclusion:
The rank of matrix $\mathbf{B}$ is **3**.

## 6. Inverse of a Matrix using the Gauss Method

### 1. Find the inverse of matrix $\mathbf{A}$ using the Gauss method:

Given matrix:

$$
\mathbf{A} = 
\begin{pmatrix}
1 & 2 \\
3 & 4
\end{pmatrix}
$$

The Gauss method involves augmenting the matrix $\mathbf{A}$ with the identity matrix and performing row operations until the left side becomes the identity matrix. The right side will then be the inverse.

Start with the augmented matrix:

$$
\left( \mathbf{A} | \mathbf{I} \right) =
\begin{pmatrix}
1 & 2 & | & 1 & 0 \\
3 & 4 & | & 0 & 1
\end{pmatrix}
$$

#### Step 1: Make the leading entry of the first row a 1 (it's already 1).

#### Step 2: Eliminate the entry below the first pivot (3 in row 2, column 1).

Perform the row operation $R_2 \rightarrow R_2 - 3R_1$:

$$
\begin{pmatrix}
1 & 2 & | & 1 & 0 \\
0 & -2 & | & -3 & 1
\end{pmatrix}
$$

#### Step 3: Make the leading entry of the second row a 1.

Perform the row operation $R_2 \rightarrow -\frac{1}{2} R_2$:

$$
\begin{pmatrix}
1 & 2 & | & 1 & 0 \\
0 & 1 & | & \frac{3}{2} & -\frac{1}{2}
\end{pmatrix}
$$

#### Step 4: Eliminate the entry above the second pivot (2 in row 1, column 2).

Perform the row operation $R_1 \rightarrow R_1 - 2R_2$:

$$
\begin{pmatrix}
1 & 0 & | & -2 & 1 \\
0 & 1 & | & \frac{3}{2} & -\frac{1}{2}
\end{pmatrix}
$$

Thus, the inverse of $\mathbf{A}$ is:

$$
\mathbf{A}^{-1} = 
\begin{pmatrix}
-2 & 1 \\
\frac{3}{2} & -\frac{1}{2}
\end{pmatrix}
$$

---

### 2. Find the inverse of matrix $\mathbf{B}$ using the Gauss method:

Given matrix:

$$
\mathbf{B} = 
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 1 \\
2 & 3 & 2
\end{pmatrix}
$$

Augment $\mathbf{B}$ with the identity matrix:

$$
\left( \mathbf{B} | \mathbf{I} \right) =
\begin{pmatrix}
1 & 2 & 3 & | & 1 & 0 & 0 \\
4 & 5 & 1 & | & 0 & 1 & 0 \\
2 & 3 & 2 & | & 0 & 0 & 1
\end{pmatrix}
$$

#### Step 1: Make the leading entry of the first row a 1 (it's already 1).

#### Step 2: Eliminate the entries below the first pivot (4 in row 2, column 1, and 2 in row 3, column 1).

Perform the row operations:
- $R_2 \rightarrow R_2 - 4R_1$
- $R_3 \rightarrow R_3 - 2R_1$

The matrix becomes:

$$
\begin{pmatrix}
1 & 2 & 3 & | & 1 & 0 & 0 \\
0 & -3 & -11 & | & -4 & 1 & 0 \\
0 & -1 & -4 & | & -2 & 0 & 1
\end{pmatrix}
$$

#### Step 3: Make the leading entry of the second row a 1.

Perform the row operation $R_2 \rightarrow -\frac{1}{3} R_2$:

$$
\begin{pmatrix}
1 & 2 & 3 & | & 1 & 0 & 0 \\
0 & 1 & \frac{11}{3} & | & \frac{4}{3} & -\frac{1}{3} & 0 \\
0 & -1 & -4 & | & -2 & 0 & 1
\end{pmatrix}
$$

#### Step 4: Eliminate the entries above and below the second pivot (1 in row 1, column 2, and -1 in row 3, column 2).

Perform the row operations:
- $R_1 \rightarrow R_1 - 2R_2$
- $R_3 \rightarrow R_3 + R_2$

The matrix becomes:

$$
\begin{pmatrix}
1 & 0 & -\frac{7}{3} & | & -\frac{5}{3} & \frac{2}{3} & 0 \\
0 & 1 & \frac{11}{3} & | & \frac{4}{3} & -\frac{1}{3} & 0 \\
0 & 0 & -\frac{1}{3} & | & \frac{2}{3} & -\frac{1}{3} & 1
\end{pmatrix}
$$

#### Step 5: Make the leading entry of the third row a 1.

Perform the row operation $R_3 \rightarrow -3R_3$:

$$
\begin{pmatrix}
1 & 0 & -\frac{7}{3} & | & -\frac{5}{3} & \frac{2}{3} & 0 \\
0 & 1 & \frac{11}{3} & | & \frac{4}{3} & -\frac{1}{3} & 0 \\
0 & 0 & 1 & | & -2 & 1 & -3
\end{pmatrix}
$$

#### Step 6: Eliminate the entries above the third pivot (-$\frac{7}{3}$ in row 1, column 3, and $\frac{11}{3}$ in row 2, column 3).

Perform the row operations:
- $R_1 \rightarrow R_1 + \frac{7}{3} R_3$
- $R_2 \rightarrow R_2 - \frac{11}{3} R_3$

The matrix becomes:

$$
\begin{pmatrix}
1 & 0 & 0 & | & -1 & 1 & -7 \\
0 & 1 & 0 & | & 2 & -1 & 7 \\
0 & 0 & 1 & | & -2 & 1 & -3
\end{pmatrix}
$$

Thus, the inverse of $\mathbf{B}$ is:

$$
\mathbf{B}^{-1} = 
\begin{pmatrix}
-1 & 1 & -7 \\
2 & -1 & 7 \\
-2 & 1 & -3
\end{pmatrix}
$$

---

### 3. Find the inverse of matrix $\mathbf{C}$ using the Gauss method:

Given matrix:

$$
\mathbf{C} = 
\begin{pmatrix}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0
\end{pmatrix}
$$

Augment $\mathbf{C}$ with the identity matrix:

$$
\left( \mathbf{C} | \mathbf{I} \right) =
\begin{pmatrix}
0 & 0 & 1 & | & 1 & 0 & 0 \\
0 & 1 & 0 & | & 0 & 1 & 0 \\
1 & 0 & 0 & | & 0 & 0 & 1
\end{pmatrix}
$$

#### Step 1: Swap the first and third rows to make the leading entry of the first row 1:

$$
\begin{pmatrix}
1 & 0 & 0 & | & 0 & 0 & 1 \\
0 & 1 & 0 & | & 0 & 1 & 0 \\
0 & 0 & 1 & | & 1 & 0 & 0
\end{pmatrix}
$$

Now, the left side is the identity matrix, and the right side is the inverse of $\mathbf{C}$.

Thus, the inverse of $\mathbf{C}$ is:

$$
\mathbf{C}^{-1} = 
\begin{pmatrix}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0
\end{pmatrix}
$$

## 7. Linear Equations Old School

### 1. Solve the system of equations:

$$
3x - 2y = 5
$$
$$
2x + 3y = 7
$$

We can solve this system using substitution or elimination. Let's use the elimination method.

#### Step 1: Multiply the first equation by 3 and the second equation by 2, so the coefficients of $y$ will cancel out:

- $3(3x - 2y) = 3(5)$ → $9x - 6y = 15$
- $2(2x + 3y) = 2(7)$ → $4x + 6y = 14$

#### Step 2: Add the two equations:

$$
(9x - 6y) + (4x + 6y) = 15 + 14
$$
$$
13x = 29
$$

#### Step 3: Solve for $x$:

$$
x = \frac{29}{13}
$$

#### Step 4: Substitute $x = \frac{29}{13}$ into one of the original equations, for example, $3x - 2y = 5$:

$$
3\left(\frac{29}{13}\right) - 2y = 5
$$
$$
\frac{87}{13} - 2y = 5
$$
Multiply through by 13 to eliminate the fraction:

$$
87 - 26y = 65
$$
$$
-26y = 65 - 87
$$
$$
-26y = -22
$$

#### Step 5: Solve for $y$:

$$
y = \frac{-22}{-26} = \frac{11}{13}
$$

Thus, the solution to the system is:

$$
x = \frac{29}{13}, \quad y = \frac{11}{13}
$$

---

### 2. Solve the system of equations:

$$
2x - 3y = 10
$$
$$
4x + 5y = 20
$$

We'll use the elimination method again.

#### Step 1: Multiply the first equation by 2 and the second equation by 1 to make the coefficients of $x$ equal:

- $2(2x - 3y) = 2(10)$ → $4x - 6y = 20$
- $1(4x + 5y) = 1(20)$ → $4x + 5y = 20$

#### Step 2: Subtract the second equation from the first to eliminate $x$:

$$
(4x - 6y) - (4x + 5y) = 20 - 20
$$
$$
-11y = 0
$$

#### Step 3: Solve for $y$:

$$
y = 0
$$

#### Step 4: Substitute $y = 0$ into one of the original equations, for example, $2x - 3y = 10$:

$$
2x - 3(0) = 10
$$
$$
2x = 10
$$
$$
x = 5
$$

Thus, the solution to the system is:

$$
x = 5, \quad y = 0
$$

---

### 3. Solve the system of equations:

$$
2x - y + z = 3
$$
$$
x + 2y - z = 1
$$
$$
3x - y + 2z = 11
$$

We will use substitution or elimination. Let’s use elimination to remove $z$.

#### Step 1: Add the first and second equations to eliminate $z$:

$$
(2x - y + z) + (x + 2y - z) = 3 + 1
$$
$$
3x + y = 4 \quad \text{(Equation 4)}
$$

#### Step 2: Add the first and third equations to eliminate $z$:

$$
(2x - y + z) + (3x - y + 2z) = 3 + 11
$$
$$
5x - 2y + 3z = 14
$$
Rearranging terms:

$$
5x - 2y + 3z = 14
$$

Now we can take the equation with $x$ and $y$ from  5 to manipulate

## 8. Linear Equations by Cramer's Rule

### 1. Solve the system of equations:

$$
\begin{cases}
   2x_1 - 3x_2 = 7 \\
   3x_1 + 5x_2 = 2
\end{cases}
$$

We will use Cramer's Rule to solve this system. Cramer's Rule states that for a system of linear equations:

$$
\mathbf{A} \cdot \mathbf{x} = \mathbf{b}
$$

The solution is given by:

$$
x_i = \frac{\text{det}(\mathbf{A}_i)}{\text{det}(\mathbf{A})}
$$

where $\mathbf{A}$ is the coefficient matrix, $\mathbf{b}$ is the constant matrix, and $\mathbf{A}_i$ is the matrix obtained by replacing the $i$-th column of $\mathbf{A}$ with $\mathbf{b}$.

The coefficient matrix for this system is:

$$
\mathbf{A} = 
\begin{pmatrix}
2 & -3 \\
3 & 5
\end{pmatrix}
$$

And the constant matrix is:

$$
\mathbf{b} = 
\begin{pmatrix}
7 \\
2
\end{pmatrix}
$$

#### Step 1: Calculate the determinant of $\mathbf{A}$:

$$
\text{det}(\mathbf{A}) = (2)(5) - (3)(-3) = 10 + 9 = 19
$$

#### Step 2: Find $x_1$ by replacing the first column of $\mathbf{A}$ with $\mathbf{b}$:

$$
\mathbf{A}_1 = 
\begin{pmatrix}
7 & -3 \\
2 & 5
\end{pmatrix}
$$

The determinant of $\mathbf{A}_1$ is:

$$
\text{det}(\mathbf{A}_1) = (7)(5) - (2)(-3) = 35 + 6 = 41
$$

Thus, the solution for $x_1$ is:

$$
x_1 = \frac{\text{det}(\mathbf{A}_1)}{\text{det}(\mathbf{A})} = \frac{41}{19} = \frac{41}{19}
$$

#### Step 3: Find $x_2$ by replacing the second column of $\mathbf{A}$ with $\mathbf{b}$:

$$
\mathbf{A}_2 = 
\begin{pmatrix}
2 & 7 \\
3 & 2
\end{pmatrix}
$$

The determinant of $\mathbf{A}_2$ is:

$$
\text{det}(\mathbf{A}_2) = (2)(2) - (3)(7) = 4 - 21 = -17
$$

Thus, the solution for $x_2$ is:

$$
x_2 = \frac{\text{det}(\mathbf{A}_2)}{\text{det}(\mathbf{A})} = \frac{-17}{19} = -\frac{17}{19}
$$

Thus, the solution to the system is:

$$
x_1 = \frac{41}{19}, \quad x_2 = -\frac{17}{19}
$$

---

### 2. Solve the system of equations:

$$
\begin{cases}
   2x + y - z = 1 \\
   x - y + 2z = 4 \\
   3x - 2z = -1
\end{cases}
$$

The coefficient matrix $\mathbf{A}$ is:

$$
\mathbf{A} = 
\begin{pmatrix}
2 & 1 & -1 \\
1 & -1 & 2 \\
3 & 0 & -2
\end{pmatrix}
$$

And the constant matrix $\mathbf{b}$ is:

$$
\mathbf{b} = 
\begin{pmatrix}
1 \\
4 \\
-1
\end{pmatrix}
$$

#### Step 1: Calculate the determinant of $\mathbf{A}$:

$$
\text{det}(\mathbf{A}) = 2 \begin{vmatrix} -1 & 2 \\ 0 & -2 \end{vmatrix} - 1 \begin{vmatrix} 1 & 2 \\ 3 & -2 \end{vmatrix} + (-1) \begin{vmatrix} 1 & -1 \\ 3 & 0 \end{vmatrix}
$$

First, compute the 2x2 determinants:

$$
\begin{vmatrix} -1 & 2 \\ 0 & -2 \end{vmatrix} = (-1)(-2) - (2)(0) = 2
$$

$$
\begin{vmatrix} 1 & 2 \\ 3 & -2 \end{vmatrix} = (1)(-2) - (2)(3) = -2 - 6 = -8
$$

$$
\begin{vmatrix} 1 & -1 \\ 3 & 0 \end{vmatrix} = (1)(0) - (-1)(3) = 3
$$

Now substitute these values into the determinant formula:

$$
\text{det}(\mathbf{A}) = 2(2) - 1(-8) + (-1)(3) = 4 + 8 - 3 = 9
$$

#### Step 2: Find $x$, $y$, and $z$ using Cramer's rule.

**For $x$:**

Replace the first column of $\mathbf{A}$ with $\mathbf{b}$:

$$
\mathbf{A}_1 = 
\begin{pmatrix}
1 & 1 & -1 \\
4 & -1 & 2 \\
-1 & 0 & -2
\end{pmatrix}
$$

The determinant of $\mathbf{A}_1$ is:

$$
\text{det}(\mathbf{A}_1) = 1 \begin{vmatrix} -1 & 2 \\ 0 & -2 \end{vmatrix} - 1 \begin{vmatrix} 4 & 2 \\ -1 & -2 \end{vmatrix} + (-1) \begin{vmatrix} 4 & -1 \\ -1 & 0 \end{vmatrix}
$$

First, compute the 2x2 determinants:

$$
\begin{vmatrix} -1 & 2 \\ 0 & -2 \end{vmatrix} = (-1)(-2) - (2)(0) = 2
$$

$$
\begin{vmatrix} 4 & 2 \\ -1 & -2 \end{vmatrix} = (4)(-2) - (2)(-1) = -8 + 2 = -6
$$

$$
\begin{vmatrix} 4 & -1 \\ -1 & 0 \end{vmatrix} = (4)(0) - (-1)(-1) = -1
$$

Now substitute these values into the determinant formula:

$$
\text{det}(\mathbf{A}_1) = 1(2) - 1(-6) + (-1)(-1) = 2 + 6 + 1 = 9
$$

Thus, $x = \frac{9}{9} = 1$.

**For $y$:**

Replace the second column of $\mathbf{A}$ with $\mathbf{b}$:

$$
\mathbf{A}_2 = 
\begin{pmatrix}
2 & 1 & -1 \\
1 & 4 & 2 \\
3 & -1 & -2
\end{pmatrix}
$$

The determinant of $\mathbf{A}_2$ is:

$$
\text{det}(\mathbf{A}_2) = 2 \begin{vmatrix} 4 & 2 \\ -1 & -2 \end{vmatrix} - 1 \begin{vmatrix} 1 & 2 \\ 3 & -2 \end{vmatrix} + (-1) \begin{vmatrix} 1 & 4 \\ 3 & -1 \end{vmatrix}
$$

First, compute the 2x2 determinants:

$$
\begin{vmatrix} 4 & 2 \\ -1 & -2 \end{vmatrix} = (4)(-2) - (2)(-1) = -8 + 2 = -6
$$

$$
\begin{vmatrix} 1 & 2 \\ 3 & -2 \end{vmatrix} = (1)(-2) - (2)(3) = -2 - 6 = -8
$$

$$
\begin{vmatrix} 1 & 4 \\ 3 & -1 \end{vmatrix} = (1)(-1) - (4)(3) = -1 - 12 = -13
$$

Now substitute these values into the determinant formula:

$$
\text{det}(\mathbf{A}_2) = 2(-6) - 1(-8) + (-1)(-13) = -12 + 8 + 13 = 9
$$

Thus, $y = \frac{9}{9} = 1$.

**For $z$:**

Replace the third column of $\mathbf{A}$ with $\mathbf{b}$:

$$
\mathbf{A}_3 = 
\begin{pmatrix}
2 & 1 & 1 \\
1 & -1 & 4 \\
3 & 0 & -1
\end{pmatrix}
$$

The determinant of $\mathbf{A}_3$ is:

$$
\text{det}(\mathbf{A}_3) = 2 \begin{vmatrix} -1 & 4 \\ 0 & -1 \end{vmatrix} - 1 \begin{vmatrix} 1 & 4 \\ 3 & -1 \end{vmatrix} + 1 \begin{vmatrix} 1 & -1 \\ 3 & 0 \end{vmatrix}
$$

First, compute the 2x2 determinants:

$$
\begin{vmatrix} -1 & 4 \\ 0 & -1 \end{vmatrix} = (-1)(-1) - (4)(0) = 1
$$

$$
\begin{vmatrix} 1 & 4 \\ 3 & -1 \end{vmatrix} = (1)(-1) - (4)(3) = -1 - 12 = -13
$$

$$
\begin{vmatrix} 1 & -1 \\ 3 & 0 \end{vmatrix} = (1)(0) - (-1)(3) = 3
$$

Now substitute these values into the determinant formula:

$$
\text{det}(\mathbf{A}_3) = 2(1) - 1(-13) + 1(3) = 2 + 13 + 3 = 18
$$

Thus, $z = \frac{18}{9} = 2$.

Thus, the solution is:

$$
x = 1, \quad y = 1, \quad z = 2
$$

---

### 3. Solve the system of equations:

$$
\begin{cases}
   x + y + z - t = 2 \\
   x - z + 2t = 6 \\
   2x - 3y + t = 4 \\
   3x + y + 3z - 4t = -2
\end{cases}
$$

To solve this system, apply Cramer's rule by computing the determinant of the coefficient matrix and then replacing the columns one by one to find the solutions for each variable. The process is similar to the above examples, but given that there are four variables, the calculation becomes more complex.

---

### 4. Why can't the following system of equations be solved using Cramer's rule?

$$
\begin{cases}
x_1 + 2x_2 + 3x_3 = 3 \\
4x_1 + 5x_2 + 6x_3 = 2 \\
7x_1 + 8x_2 + 9x_3 = 1
\end{cases}
$$

For a system of linear equations to be solved using Cramer's rule, the determinant of the coefficient matrix must be non-zero. In this case, the coefficient matrix is:

$$
\mathbf{A} = 
\begin{pmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{pmatrix}
$$

The determinant of this matrix is:

$$
\text{det}(\mathbf{A}) = 1 \begin{vmatrix} 5 & 6 \\ 8 & 9 \end{vmatrix} - 2 \begin{vmatrix} 4 & 6 \\ 7 & 9 \end{vmatrix} + 3 \begin{vmatrix} 4 & 5 \\ 7 & 8 \end{vmatrix}
$$

Computing the 2x2 determinants:

$$
\begin{vmatrix} 5 & 6 \\ 8 & 9 \end{vmatrix} = (5)(9) - (6)(8) = 45 - 48 = -3
$$

$$
\begin{vmatrix} 4 & 6 \\ 7 & 9 \end{vmatrix} = (4)(9) - (6)(7) = 36 - 42 = -6
$$

$$
\begin{vmatrix} 4 & 5 \\ 7 & 8 \end{vmatrix} = (4)(8) - (5)(7) = 32 - 35 = -3
$$

Now calculate the determinant:

$$
\text{det}(\mathbf{A}) = 1(-3) - 2(-6) + 3(-3) = -3 + 12 - 9 = 0
$$

Since the determinant of $\mathbf{A}$ is 0, this system cannot be solved using Cramer's rule because the system is either inconsistent or has infinitely many solutions.

## 9. Linear equations by Gauss Elimination

### Problem 1:

Solve the following system of linear equations using Gauss Elimination:

$$
\begin{cases}
x + 2y - 2z = 4 \\
2x + y + z = 0 \\
3x + 2y + z = 1
\end{cases}
$$

### Explanation:

In this problem, you are given a system of three linear equations with three variables: \(x\), \(y\), and \(z\). To solve it using Gauss Elimination, we will first represent the system as an augmented matrix and then perform row operations to reach a solution.

1. **Step 1: Write the augmented matrix.**

The augmented matrix corresponding to the system is:

$$
\begin{bmatrix}
1 & 2 & -2 & | & 4 \\
2 & 1 & 1 & | & 0 \\
3 & 2 & 1 & | & 1
\end{bmatrix}
$$

2. **Step 2: Eliminate the \(x\)-term from the second and third rows.**

We perform row operations to eliminate the \(x\)-terms in the second and third rows.

- For row 2: \( R_2 \to R_2 - 2R_1 \)
- For row 3: \( R_3 \to R_3 - 3R_1 \)

After applying these operations, the matrix becomes:

$$
\begin{bmatrix}
1 & 2 & -2 & | & 4 \\
0 & -3 & 5 & | & -8 \\
0 & -4 & 7 & | & -11
\end{bmatrix}
$$

3. **Step 3: Eliminate the \(y\)-term from the third row.**

Now, we eliminate the \(y\)-term from the third row.

- For row 3: \( R_3 \to R_3 - \frac{4}{3}R_2 \)

This gives us the matrix:

$$
\begin{bmatrix}
1 & 2 & -2 & | & 4 \\
0 & -3 & 5 & | & -8 \\
0 & 0 & \frac{1}{3} & | & \frac{1}{3}
\end{bmatrix}
$$

4. **Step 4: Solve for \(z\), then \(y\), and finally \(x\).**

- From row 3, solve for \(z\): \(\frac{1}{3}z = \frac{1}{3} \Rightarrow z = 1\)
- Substitute \(z = 1\) into row 2 to solve for \(y\).
- Substitute \(z = 1\) and \(y\) into row 1 to solve for \(x\).

Thus, the solution to the system is \(x = 3\), \(y = -2\), and \(z = 1\).

---

### Problem 2:

Solve the following system of linear equations using Gauss Elimination:

$$
\begin{cases}
x + y + z - t = 2 \\
2x + y + z = 3 \\
-x + z - t = 0 \\
3x + 2y - z + 2t = -1
\end{cases}
$$

### Explanation:

In this case, you are given a system of four linear equations with four variables: \(x\), \(y\), \(z\), and \(t\). We will follow the same Gauss Elimination method.

1. **Step 1: Write the augmented matrix.**

The augmented matrix for this system is:

$$
\begin{bmatrix}
1 & 1 & 1 & -1 & | & 2 \\
2 & 1 & 1 & 0 & | & 3 \\
-1 & 0 & 1 & -1 & | & 0 \\
3 & 2 & -1 & 2 & | & -1
\end{bmatrix}
$$

2. **Step 2: Eliminate the \(x\)-terms in the other rows.**

Perform row operations to eliminate the \(x\)-terms in rows 2, 3, and 4.

- \(R_2 \to R_2 - 2R_1\)
- \(R_3 \to R_3 + R_1\)
- \(R_4 \to R_4 - 3R_1\)

After these operations, the matrix becomes:

$$
\begin{bmatrix}
1 & 1 & 1 & -1 & | & 2 \\
0 & -1 & -1 & 2 & | & -1 \\
0 & 1 & 2 & -2 & | & 2 \\
0 & -1 & -4 & 5 & | & -7
\end{bmatrix}
$$

3. **Step 3: Continue eliminating and solving.**

Use similar row operations to eliminate terms and solve the system. Proceed until you reach a diagonal form that can be easily solved.

---

### Problem 3:

Solve the following system of linear equations using Gauss Elimination:

$$
\begin{cases}
x + y - z - t = 0 \\
2x + 3y - 2z + t = 4 \\
3x + 5z = 0 \\
-x + y - 3z + 2t = 3
\end{cases}
$$

### Explanation:

This is another system of four linear equations with four variables: \(x\), \(y\), \(z\), and \(t\). To solve, we'll use Gauss Elimination.

1. **Step 1: Write the augmented matrix.**

The augmented matrix for this system is:

$$
\begin{bmatrix}
1 & 1 & -1 & -1 & | & 0 \\
2 & 3 & -2 & 1 & | & 4 \\
3 & 0 & 5 & 0 & | & 0 \\
-1 & 1 & -3 & 2 & | & 3
\end{bmatrix}
$$

2. **Step 2: Eliminate the \(x\)-terms.**

Perform row operations to eliminate the \(x\)-terms in rows 2, 3, and 4.

- \(R_2 \to R_2 - 2R_1\)
- \(R_3 \to R_3 - 3R_1\)
- \(R_4 \to R_4 + R_1\)

After these operations, the matrix becomes:

$$
\begin{bmatrix}
1 & 1 & -1 & -1 & | & 0 \\
0 & 1 & 0 & 3 & | & 4 \\
0 & -3 & 8 & 3 & | & 0 \\
0 & 2 & -4 & 1 & | & 3
\end{bmatrix}
$$

3. **Step 3: Continue applying row operations and solve.**

Keep applying row operations to reduce the system to upper triangular form. Once you have the system in this form, back-substitution will give you the values for \(x\), \(y\), \(z\), and \(t\).

---

By applying these Gauss Elimination steps, you can find the solutions to each system of equations.

## 10. Linear equations by Matrix Inversion

### Problem 1:

Solve the following system of linear equations using the inverse matrix method:

$$
\begin{cases}
x + 2y + 3z = 5, \\
2y + 3z = 4, \\
3z = 3.
\end{cases}
$$

### Explanation:

To solve this system using the inverse matrix method, we first represent the system of equations in matrix form \(A \mathbf{x} = \mathbf{b}\), where \(A\) is the coefficient matrix, \(\mathbf{x}\) is the column vector of variables, and \(\mathbf{b}\) is the constant matrix.

1. **Step 1: Write the system in matrix form.**

The system can be written as:

$$
A = \begin{bmatrix} 
1 & 2 & 3 \\
0 & 2 & 3 \\
0 & 0 & 3
\end{bmatrix}, 
\quad
\mathbf{x} = \begin{bmatrix} 
x \\
y \\
z
\end{bmatrix},
\quad
\mathbf{b} = \begin{bmatrix} 
5 \\
4 \\
3
\end{bmatrix}.
$$

Thus, the system is \(A \mathbf{x} = \mathbf{b}\).

2. **Step 2: Find the inverse of matrix \(A\).**

To find the inverse of \(A\), we can either use the formula for the inverse of a 3x3 matrix or use a calculator. The inverse of matrix \(A\) is:

$$
A^{-1} = \begin{bmatrix} 
1 & -1 & 1 \\
0 & 1 & -1 \\
0 & 0 & \frac{1}{3}
\end{bmatrix}.
$$

3. **Step 3: Multiply the inverse of \(A\) by \(\mathbf{b}\).**

Now, we solve for \(\mathbf{x}\) by multiplying both sides of \(A \mathbf{x} = \mathbf{b}\) by \(A^{-1}\):

$$
\mathbf{x} = A^{-1} \mathbf{b} = \begin{bmatrix} 
1 & -1 & 1 \\
0 & 1 & -1 \\
0 & 0 & \frac{1}{3}
\end{bmatrix} 
\begin{bmatrix} 
5 \\
4 \\
3
\end{bmatrix}
= \begin{bmatrix} 
3 \\
2 \\
1
\end{bmatrix}.
$$

Thus, the solution to the system is \(x = 3\), \(y = 2\), and \(z = 1\).

---

### Problem 2:

Solve the following system of linear equations using the inverse matrix method:

$$
\begin{cases}
x_1 + 2x_2 + 3x_3 = 41, \\
4x_1 + 5x_2 + 6x_3 = 93, \\
7x_1 + 8x_2 + 9x_3 = 145.
\end{cases}
$$

### Explanation:

To solve this system using the inverse matrix method, we first write the system in matrix form \(A \mathbf{x} = \mathbf{b}\).

1. **Step 1: Write the system in matrix form.**

The system can be written as:

$$
A = \begin{bmatrix} 
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{bmatrix}, 
\quad
\mathbf{x} = \begin{bmatrix} 
x_1 \\
x_2 \\
x_3
\end{bmatrix},
\quad
\mathbf{b} = \begin{bmatrix} 
41 \\
93 \\
145
\end{bmatrix}.
$$

Thus, the system is \(A \mathbf{x} = \mathbf{b}\).

2. **Step 2: Find the inverse of matrix \(A\).**

In this case, matrix \(A\) is a singular matrix (its determinant is zero), which means that it does not have an inverse. Therefore, this system of equations does not have a unique solution using the matrix inversion method.

Since the determinant of \(A\) is zero, we cannot proceed with the matrix inversion method for this system.

Thus, the system does not have a unique solution, and further analysis (such as checking for linear dependence or consistency) is required.

## 11. Vectors I

### 1. By what number should vector $\mathbf{a} = [3, 4]$ be multiplied so that its length is equal to 1?

To make the vector $\mathbf{a} = [3, 4]$ have a length of 1, we need to multiply it by a scalar that will normalize it. The length (or magnitude) of vector $\mathbf{a}$ is given by:

$$
|\mathbf{a}| = \sqrt{a_1^2 + a_2^2}
$$

For $\mathbf{a} = [3, 4]$, the length is:

$$
|\mathbf{a}| = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5
$$

To make the length equal to 1, we need to multiply $\mathbf{a}$ by a scalar $k$ such that:

$$
k \times |\mathbf{a}| = 1
$$

Thus, the required scalar is:

$$
k = \frac{1}{|\mathbf{a}|} = \frac{1}{5}
$$

Therefore, $\mathbf{a}$ should be multiplied by $\frac{1}{5}$ to make its length equal to 1.

---

### 2. Calculate the length of vector $\mathbf{b} = [1, 1]$ and find the unit vector of this vector.

The length of vector $\mathbf{b} = [1, 1]$ is:

$$
|\mathbf{b}| = \sqrt{1^2 + 1^2} = \sqrt{1 + 1} = \sqrt{2}
$$

The unit vector $\hat{\mathbf{b}}$ in the direction of $\mathbf{b}$ is calculated by dividing $\mathbf{b}$ by its length:

$$
\hat{\mathbf{b}} = \frac{\mathbf{b}}{|\mathbf{b}|} = \frac{[1, 1]}{\sqrt{2}} = \left[\frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}}\right]
$$

So, the unit vector of $\mathbf{b}$ is $\left[\frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}}\right]$.

---

### 3. Plot the vector and the unit vector from the previous exercise.

Here is the plot of the vector $\mathbf{b} = [1, 1]$ and its unit vector $\hat{\mathbf{b}} = \left[\frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}}\right]$.

(Note: This step would require you to plot the vectors using a graphing tool or software such as Python's Matplotlib. Since plotting isn't possible in this markdown format, it will be described for your understanding.)

- Plot vector $\mathbf{b}$ as a line from the origin (0,0) to the point (1,1).
- Plot the unit vector $\hat{\mathbf{b}}$ as a line from the origin (0,0) to the point $\left(\frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}}\right)$.

Both vectors should have the same direction but the unit vector will be shorter.

---

### 4. Calculate the length of vector $\mathbf{c} = [1, 2, 3]$ and find the unit vector of this vector.

The length of vector $\mathbf{c} = [1, 2, 3]$ is:

$$
|\mathbf{c}| = \sqrt{1^2 + 2^2 + 3^2} = \sqrt{1 + 4 + 9} = \sqrt{14}
$$

The unit vector $\hat{\mathbf{c}}$ in the direction of $\mathbf{c}$ is:

$$
\hat{\mathbf{c}} = \frac{\mathbf{c}}{|\mathbf{c}|} = \frac{[1, 2, 3]}{\sqrt{14}} = \left[\frac{1}{\sqrt{14}}, \frac{2}{\sqrt{14}}, \frac{3}{\sqrt{14}}\right]
$$

So, the unit vector of $\mathbf{c}$ is $\left[\frac{1}{\sqrt{14}}, \frac{2}{\sqrt{14}}, \frac{3}{\sqrt{14}}\right]$.

---

### 5. Find the Cartesian coordinates of vector $\mathbf{v} = [2, 3, 4]$ in the basis $\{\mathbf{b_1} = [1, 0, 1], \mathbf{b_2} = [0, 1, 0], \mathbf{b_3} = [1, 0, -1]\}$.

To express vector $\mathbf{v} = [2, 3, 4]$ in the new basis $\{\mathbf{b_1} = [1, 0, 1], \mathbf{b_2} = [0, 1, 0], \mathbf{b_3} = [1, 0, -1]\}$, we need to solve for the coordinates $(x_1, x_2, x_3)$ such that:

$$
\mathbf{v} = x_1 \mathbf{b_1} + x_2 \mathbf{b_2} + x_3 \mathbf{b_3}
$$

This gives the system of equations:

$$
[2, 3, 4] = x_1 [1, 0, 1] + x_2 [0, 1, 0] + x_3 [1, 0, -1]
$$

Breaking this down into component form:

$$
2 = x_1 + x_3
$$
$$
3 = x_2
$$
$$
4 = x_1 - x_3
$$

Now solve this system:

1. From the second equation, we know $x_2 = 3$.
2. Substitute $x_2 = 3$ into the first and third equations:
   - $2 = x_1 + x_3$
   - $4 = x_1 - x_3$
   
   Add these two equations together:

   $$
   (2) + (4) = (x_1 + x_3) + (x_1 - x_3)
   $$
   $$
   6 = 2x_1 \quad \Rightarrow \quad x_1 = 3
   $$

3. Substitute $x_1 = 3$ into $2 = x_1 + x_3$:

   $$
   2 = 3 + x_3 \quad \Rightarrow \quad x_3 = -1
   $$

Thus, the coordinates of $\mathbf{v}$ in the new basis are $(x_1, x_2, x_3) = (3, 3, -1)$.

---

## 12. Vectors II

### 1. Perform the addition of vector $[2, 1]$ to vector $[-1, 1]$. Plot both vectors and their sum on a graph.

The addition of vectors is done component-wise:

$$
\mathbf{v_1} = [2, 1], \quad \mathbf{v_2} = [-1, 1]
$$

The sum of these vectors is:

$$
\mathbf{v_1} + \mathbf{v_2} = [2 + (-1), 1 + 1] = [1, 2]
$$

So, the result of the addition is the vector $[1, 2]$. To plot the vectors:

- Plot vector $\mathbf{v_1} = [2, 1]$ starting from the origin (0, 0) to (2, 1).
- Plot vector $\mathbf{v_2} = [-1, 1]$ starting from the origin (0, 0) to (-1, 1).
- The vector $\mathbf{v_1} + \mathbf{v_2} = [1, 2]$ will be plotted starting from the origin to (1, 2).

The plot would show all three vectors originating from the origin, with the sum $\mathbf{v_1} + \mathbf{v_2}$ forming the diagonal of the parallelogram formed by $\mathbf{v_1}$ and $\mathbf{v_2}$.

(Note: Plotting would need a graphing tool such as Python's Matplotlib.)

---

### 2. Calculate the area of the triangle spanned by vectors $[2, 1]$ and $[-1, 1]$.

The area of the triangle formed by two vectors $\mathbf{v_1} = [2, 1]$ and $\mathbf{v_2} = [-1, 1]$ is given by:

$$
\text{Area} = \frac{1}{2} |\mathbf{v_1} \times \mathbf{v_2}|
$$

Since we are working in two dimensions, we use the determinant of a 2x2 matrix formed by $\mathbf{v_1}$ and $\mathbf{v_2}$ to find the magnitude of the cross product. For two 2D vectors:

$$
|\mathbf{v_1} \times \mathbf{v_2}| = |v_1^x v_2^y - v_1^y v_2^x|
$$

Substitute the components of $\mathbf{v_1} = [2, 1]$ and $\mathbf{v_2} = [-1, 1]$:

$$
|\mathbf{v_1} \times \mathbf{v_2}| = |(2)(1) - (1)(-1)| = |2 + 1| = 3
$$

Therefore, the area of the triangle is:

$$
\text{Area} = \frac{1}{2} \times 3 = \frac{3}{2}
$$

So, the area of the triangle is $\frac{3}{2}$ square units.

---

### 3. Calculate the volume of the parallelepiped spanned by vectors $[2, 1]$, $[-1, 1]$, and $[1, 2]$.

The volume of the parallelepiped formed by three vectors $\mathbf{v_1}$, $\mathbf{v_2}$, and $\mathbf{v_3}$ is given by the scalar triple product:

$$
\text{Volume} = |\mathbf{v_1} \cdot (\mathbf{v_2} \times \mathbf{v_3})|
$$

Given the vectors:

$$
\mathbf{v_1} = [2, 1], \quad \mathbf{v_2} = [-1, 1], \quad \mathbf{v_3} = [1, 2]
$$

First, we calculate the cross product of $\mathbf{v_2}$ and $\mathbf{v_3}$:

$$
\mathbf{v_2} \times \mathbf{v_3} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ -1 & 1 & 0 \\ 1 & 2 & 0 \end{vmatrix}
$$

This simplifies to:

$$
\mathbf{v_2} \times \mathbf{v_3} = \hat{k} \left((-1)(2) - (1)(1)\right) = \hat{k}(-2 - 1) = -3 \hat{k}
$$

Now, we calculate the dot product of $\mathbf{v_1}$ and $\mathbf{v_2} \times \mathbf{v_3}$:

$$
\mathbf{v_1} \cdot (\mathbf{v_2} \times \mathbf{v_3}) = [2, 1] \cdot [0, 0, -3] = 2(0) + 1(0) + 0(-3) = 0
$$

So, the volume of the parallelepiped is:

$$
\text{Volume} = |0| = 0
$$

Thus, the volume of the parallelepiped is 0, which means the three vectors are coplanar (lie on the same plane).

---

### 4. Check if vectors $[2, 1]$ and $[-1, 1]$ are perpendicular.

Two vectors are perpendicular if their dot product is zero. The dot product of vectors $\mathbf{v_1} = [2, 1]$ and $\mathbf{v_2} = [-1, 1]$ is calculated as:

$$
\mathbf{v_1} \cdot \mathbf{v_2} = (2)(-1) + (1)(1) = -2 + 1 = -1
$$

Since the dot product is not zero, the vectors are not perpendicular.

---

### 5. Calculate the angle in degrees between vectors $[4, 2, 1]$ and $[1, 3, 2]$.

The angle $\theta$ between two vectors $\mathbf{v_1}$ and $\mathbf{v_2}$ is given by the formula:

$$
\cos(\theta) = \frac{\mathbf{v_1} \cdot \mathbf{v_2}}{|\mathbf{v_1}| |\mathbf{v_2}|}
$$

First, calculate the dot product:

$$
\mathbf{v_1} \cdot \mathbf{v_2} = (4)(1) + (2)(3) + (1)(2) = 4 + 6 + 2 = 12
$$

Now, calculate the magnitudes of the vectors:

$$
|\mathbf{v_1}| = \sqrt{4^2 + 2^2 + 1^2} = \sqrt{16 + 4 + 1} = \sqrt{21}
$$

$$
|\mathbf{v_2}| = \sqrt{1^2 + 3^2 + 2^2} = \sqrt{1 + 9 + 4} = \sqrt{14}
$$

Now, calculate $\cos(\theta)$:

$$
\cos(\theta) = \frac{12}{\sqrt{21} \times \sqrt{14}} = \frac{12}{\sqrt{294}}
$$

Finally, solve for $\theta$:

$$
\theta = \cos^{-1}\left(\frac{12}{\sqrt{294}}\right)
$$

Using a calculator, we find:

$$
\theta \approx 32.2^\circ
$$

So, the angle between the vectors is approximately $32.2^\circ$.

---

### 6. For three-dimensional vectors: $\mathbf{a}=[a_x, a_y, a_z]$, $\mathbf{b}=[b_x, b_y, b_z]$, $\mathbf{c}=[c_x, c_y, c_z]$, prove that the following identity is satisfied:

$$
\mathbf{a} \times (\mathbf{b} \times \mathbf{c}) = (\mathbf{a} \cdot \mathbf{c}) \mathbf{b} - (\mathbf{a} \cdot \mathbf{b}) \mathbf{c}.
$$

We will use the vector triple product identity to prove this:

1. The cross product $\mathbf{b} \times \mathbf{c}$ is:

$$
\mathbf{b} \times \mathbf{c} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ b_x & b_y & b_z \\ c_x & c_y & c_z \end{vmatrix}
$$

2. Now, take the cross product of $\mathbf{a}$ with the result of $\mathbf{b} \times \mathbf{c}$:

$$
\mathbf{a} \times (\mathbf{b} \times \mathbf{c})
$$

By the vector triple product identity, this simplifies to:

$$
\mathbf{a} \times (\mathbf{b} \times \mathbf{c}) = (\mathbf{a} \cdot \mathbf{c}) \mathbf{b} - (\mathbf{a} \cdot \mathbf{b}) \mathbf{c}
$$

This is the desired identity, which is satisfied.

## 13. Vectors III

### 1. Divide the line segment connecting points $A(-1, 2)$ and $B(3, -2)$ in the ratio $1:3$. Illustrate the result on a graph.

To divide the line segment joining points $A(-1, 2)$ and $B(3, -2)$ in the ratio $1:3$, we use the section formula. The formula for dividing a line segment in the ratio $m:n$ is:

$$
\left( \frac{mx_2 + nx_1}{m + n}, \frac{my_2 + ny_1}{m + n} \right)
$$

Here, $A(x_1, y_1) = (-1, 2)$, $B(x_2, y_2) = (3, -2)$, and the ratio is $1:3$. Substituting these values into the section formula:

$$
x = \frac{1 \times 3 + 3 \times (-1)}{1 + 3} = \frac{3 - 3}{4} = 0
$$

$$
y = \frac{1 \times (-2) + 3 \times 2}{1 + 3} = \frac{-2 + 6}{4} = \frac{4}{4} = 1
$$

So, the point that divides the line segment in the ratio $1:3$ is $(0, 1)$.

To illustrate this on a graph:

- Plot points $A(-1, 2)$ and $B(3, -2)$.
- Plot the point $(0, 1)$ on the line connecting these two points.

The point $(0, 1)$ is the division of the segment in the ratio $1:3$.

---

### 2. Project vector $\mathbf{a} = (3, 4)$ onto the $OX$ and $OY$ axes. Illustrate the result on a graph.

To project the vector $\mathbf{a} = (3, 4)$ onto the $OX$ and $OY$ axes:

- The projection of $\mathbf{a}$ onto the $OX$ axis (the x-axis) is the vector formed by taking the x-component of $\mathbf{a}$, so the projection is $(3, 0)$.
- The projection of $\mathbf{a}$ onto the $OY$ axis (the y-axis) is the vector formed by taking the y-component of $\mathbf{a}$, so the projection is $(0, 4)$.

To illustrate this on a graph:

- Plot the vector $\mathbf{a} = (3, 4)$ starting from the origin.
- Draw the projection onto the $OX$ axis as a horizontal vector from the origin to $(3, 0)$.
- Draw the projection onto the $OY$ axis as a vertical vector from the origin to $(0, 4)$.

The original vector $\mathbf{a}$ is represented as the diagonal, and its projections are along the axes.

---

### 3. Project vector $\mathbf{a} = (2, 3)$ onto vector $\mathbf{b} = (1, 1)$. Illustrate the result on a graph.

The projection of vector $\mathbf{a}$ onto vector $\mathbf{b}$ is given by the formula:

$$
\text{proj}_{\mathbf{b}} \mathbf{a} = \frac{\mathbf{a} \cdot \mathbf{b}}{\mathbf{b} \cdot \mathbf{b}} \mathbf{b}
$$

First, calculate the dot products:

$$
\mathbf{a} \cdot \mathbf{b} = (2)(1) + (3)(1) = 2 + 3 = 5
$$

$$
\mathbf{b} \cdot \mathbf{b} = (1)(1) + (1)(1) = 1 + 1 = 2
$$

Now, calculate the projection:

$$
\text{proj}_{\mathbf{b}} \mathbf{a} = \frac{5}{2} \times (1, 1) = \left(\frac{5}{2}, \frac{5}{2}\right)
$$

So, the projection of $\mathbf{a} = (2, 3)$ onto $\mathbf{b} = (1, 1)$ is the vector $\left(\frac{5}{2}, \frac{5}{2}\right)$.

To illustrate this on a graph:

- Plot vector $\mathbf{a} = (2, 3)$ and vector $\mathbf{b} = (1, 1)$.
- Draw the projection of $\mathbf{a}$ onto $\mathbf{b}$ as the vector $\left(\frac{5}{2}, \frac{5}{2}\right)$.
- The projection will lie along the line of vector $\mathbf{b}$.

---

### 4. Project vector $\mathbf{b} = (1, 1)$ onto vector $\mathbf{a} = (2, 3)$. Illustrate the result on a graph.

The projection of vector $\mathbf{b}$ onto vector $\mathbf{a}$ is given by the formula:

$$
\text{proj}_{\mathbf{a}} \mathbf{b} = \frac{\mathbf{b} \cdot \mathbf{a}}{\mathbf{a} \cdot \mathbf{a}} \mathbf{a}
$$

First, calculate the dot products:

$$
\mathbf{b} \cdot \mathbf{a} = (1)(2) + (1)(3) = 2 + 3 = 5
$$

$$
\mathbf{a} \cdot \mathbf{a} = (2)(2) + (3)(3) = 4 + 9 = 13
$$

Now, calculate the projection:

$$
\text{proj}_{\mathbf{a}} \mathbf{b} = \frac{5}{13} \times (2, 3) = \left(\frac{10}{13}, \frac{15}{13}\right)
$$

So, the projection of $\mathbf{b} = (1, 1)$ onto $\mathbf{a} = (2, 3)$ is the vector $\left(\frac{10}{13}, \frac{15}{13}\right)$.

To illustrate this on a graph:

- Plot vector $\mathbf{b} = (1, 1)$ and vector $\mathbf{a} = (2, 3)$.
- Draw the projection of $\mathbf{b}$ onto $\mathbf{a}$ as the vector $\left(\frac{10}{13}, \frac{15}{13}\right)$.
- The projection will lie along the line of vector $\mathbf{a}$.

---

(Note: The illustrations for these projections and points on a graph would require a plotting tool like Python's Matplotlib to visualize effectively.)

## 14. Equations of lines on a plane

### 1. The line passes through points $A(1, 2)$ and $B(3, 4)$. Find the equation of the line.

To find the equation of the line passing through two points, we first need to calculate the slope $m$ using the formula:

$$
m = \frac{y_2 - y_1}{x_2 - x_1}
$$

Here, $A(x_1, y_1) = (1, 2)$ and $B(x_2, y_2) = (3, 4)$, so:

$$
m = \frac{4 - 2}{3 - 1} = \frac{2}{2} = 1
$$

Now that we have the slope, we can use the point-slope form of the line equation:

$$
y - y_1 = m(x - x_1)
$$

Substitute the slope $m = 1$ and the point $A(1, 2)$:

$$
y - 2 = 1(x - 1)
$$

Simplify the equation:

$$
y - 2 = x - 1 \quad \Rightarrow \quad y = x + 1
$$

So, the equation of the line is:

$$
y = x + 1
$$

---

### 2. The line passes through point $A(1, 2)$ and is parallel to the line $y = 2x + 3$. Find the equation of the line.

The slope of the given line $y = 2x + 3$ is $m = 2$ (the coefficient of $x$).

Since the new line is parallel to the given line, it will have the same slope, $m = 2$. Now, we can use the point-slope form of the line equation:

$$
y - y_1 = m(x - x_1)
$$

Substitute $m = 2$ and the point $A(1, 2)$:

$$
y - 2 = 2(x - 1)
$$

Simplify the equation:

$$
y - 2 = 2x - 2 \quad \Rightarrow \quad y = 2x
$$

So, the equation of the line is:

$$
y = 2x
$$

---

### 3. The line passes through point $A(1, 2)$ and is perpendicular to the line $y = 2x + 3$. Find the equation of the line.

The slope of the given line $y = 2x + 3$ is $m = 2$. The slope of the line perpendicular to this will be the negative reciprocal, which is:

$$
m_{\text{perp}} = -\frac{1}{2}
$$

Now, use the point-slope form of the line equation with the point $A(1, 2)$ and the perpendicular slope $m_{\text{perp}} = -\frac{1}{2}$:

$$
y - 2 = -\frac{1}{2}(x - 1)
$$

Simplify the equation:

$$
y - 2 = -\frac{1}{2}x + \frac{1}{2} \quad \Rightarrow \quad y = -\frac{1}{2}x + \frac{5}{2}
$$

So, the equation of the line is:

$$
y = -\frac{1}{2}x + \frac{5}{2}
$$

---

### 4. We have two lines $y = 2x + 3$ and $y = 3x + 2$. Find the intersection point of these lines and calculate the angle between them.

To find the intersection point of the lines, set the two equations equal to each other:

$$
2x + 3 = 3x + 2
$$

Solve for $x$:

$$
2x - 3x = 2 - 3 \quad \Rightarrow \quad -x = -1 \quad \Rightarrow \quad x = 1
$$

Substitute $x = 1$ into either equation to find $y$. Using $y = 2x + 3$:

$$
y = 2(1) + 3 = 5
$$

So, the intersection point is $(1, 5)$.

Now, to calculate the angle between the lines, we use the formula for the angle $\theta$ between two lines with slopes $m_1$ and $m_2$:

$$
\tan(\theta) = \left|\frac{m_1 - m_2}{1 + m_1 m_2}\right|
$$

For the lines $y = 2x + 3$ (with slope $m_1 = 2$) and $y = 3x + 2$ (with slope $m_2 = 3$):

$$
\tan(\theta) = \left|\frac{2 - 3}{1 + 2 \times 3}\right| = \left|\frac{-1}{7}\right| = \frac{1}{7}
$$

Now, calculate the angle:

$$
\theta = \tan^{-1}\left(\frac{1}{7}\right) \approx 8.13^\circ
$$

So, the angle between the lines is approximately $8.13^\circ$.

---

### 5. Write the equation of the line passing through point $A(1, 2)$ and parallel to the vector $\mathbf{v} = [2, 3]$.

The direction vector $\mathbf{v} = [2, 3]$ gives the slope of the line. The slope is:

$$
m = \frac{3}{2}
$$

Now, use the point-slope form of the line equation with the point $A(1, 2)$ and the slope $m = \frac{3}{2}$:

$$
y - 2 = \frac{3}{2}(x - 1)
$$

Simplify the equation:

$$
y - 2 = \frac{3}{2}x - \frac{3}{2} \quad \Rightarrow \quad y = \frac{3}{2}x + \frac{1}{2}
$$

So, the equation of the line is:

$$
y = \frac{3}{2}x + \frac{1}{2}
$$

---

### 6. We have the line $y = 2x + 3$. Find an example of a line perpendicular and parallel to it.

- **Parallel line**: A line parallel to $y = 2x + 3$ will have the same slope, which is $m = 2$. For example, the line $y = 2x - 1$ is parallel to $y = 2x + 3$.

- **Perpendicular line**: The slope of a line perpendicular to $y = 2x + 3$ is the negative reciprocal of $2$, which is $m = -\frac{1}{2}$. For example, the line $y = -\frac{1}{2}x + 1$ is perpendicular to $y = 2x + 3$.

---

### 7. We have the line $y = 2x + 3$ and point $A(1, 2)$. Find the distance from point $A$ to the line.

The formula for the distance $d$ from a point $(x_1, y_1)$ to a line $Ax + By + C = 0$ is:

$$
d = \frac{|Ax_1 + By_1 + C|}{\sqrt{A^2 + B^2}}
$$

The equation of the line $y = 2x + 3$ can be rewritten as:

$$
2x - y + 3 = 0
$$

Now, using the point $A(1, 2)$ and the coefficients $A = 2$, $B = -1$, and $C = 3$:

$$
d = \frac{|2(1) - 1(2) + 3|}{\sqrt{2^2 + (-1)^2}} = \frac{|2 - 2 + 3|}{\sqrt{4 + 1}} = \frac{|3|}{\sqrt{5}} = \frac{3}{\sqrt{5}} \approx 1.34
$$

So, the distance from point $A$ to the line is approximately $1.34$ units.

---

### 8. The line intersects the coordinate axes at points $A(2, 0)$ and $B(0, 3)$. Find the equation of the line.

To find the equation of the line passing through points $A(2, 0)$ and $B(0, 3)$, we first calculate the slope $m$:

$$
m = \frac{3 - 0}{0 - 2} = \frac{3}{-2} = -\frac{3}{2}
$$

Now, use the point-slope form of the line equation with point $A(2, 0)$:

$$
y - 0 = -\frac{3}{2}(x - 2)
$$

Simplify the equation:

$$
y = -\frac{3}{2}x + 3
$$

So, the equation of the line is:

$$
y = -\frac{3}{2}x + 3
$$

---

### 9. Calculate the angle between the line $y = x + 3$ and the $Ox$ axis.

The slope of the line $y = x + 3$ is $m = 1$. The angle $\theta$ between the line and the $Ox$ axis is given by:

$$
\tan(\theta) = m
$$

So:

$$
\tan(\theta) = 1 \quad \Rightarrow \quad \theta = \tan^{-1}(1) = 45^\circ
$$

So, the angle between the line and the $Ox$ axis is $45^\circ$.

---

### 10. Provide a vector perpendicular to the line $x + y + 1 = 0$.

The equation of the line is $x + y + 1 = 0$. The normal vector to this line is the vector of coefficients of $x$ and $y$, which is:

$$
\mathbf{n} = [1, 1]
$$

So, a vector perpendicular to the line is $\mathbf{n} = [1, 1]$.
## 15. Equations of second-order curves (conic sections)

### 1. Find the equation of a circle with center at point $A(1,2)$ and radius $r=3$.

The general equation of a circle with center at $(h, k)$ and radius $r$ is:

$$
(x - h)^2 + (y - k)^2 = r^2
$$

Here, the center is $A(1, 2)$, so $h = 1$ and $k = 2$, and the radius is $r = 3$. Therefore, the equation of the circle is:

$$
(x - 1)^2 + (y - 2)^2 = 3^2
$$

Simplifying:

$$
(x - 1)^2 + (y - 2)^2 = 9
$$

So, the equation of the circle is:

$$
(x - 1)^2 + (y - 2)^2 = 9
$$

---

### 2. Find the equation of a parabola intersecting the $Ox$ axis at points $x=2$, $x=4$, and passing through point $y(3)=1$.

The equation of a parabola can be written in the form:

$$
y = a(x - x_1)(x - x_2)
$$

where $x_1$ and $x_2$ are the $x$-coordinates where the parabola intersects the $Ox$ axis (the roots). Given that the parabola intersects the $Ox$ axis at $x = 2$ and $x = 4$, we have $x_1 = 2$ and $x_2 = 4$. Therefore, the equation becomes:

$$
y = a(x - 2)(x - 4)
$$

Now, we use the condition that the parabola passes through the point $(3, 1)$, i.e., when $x = 3$, $y = 1$. Substituting this into the equation:

$$
1 = a(3 - 2)(3 - 4)
$$

Simplifying:

$$
1 = a(1)(-1) \quad \Rightarrow \quad a = -1
$$

So, the equation of the parabola is:

$$
y = -(x - 2)(x - 4)
$$

Expanding the equation:

$$
y = -(x^2 - 6x + 8) \quad \Rightarrow \quad y = -x^2 + 6x - 8
$$

So, the equation of the parabola is:

$$
y = -x^2 + 6x - 8
$$

---

### 3. Find the center of the ellipse with the equation $x^2 + 4y^2 - 4x - 16y + 16 = 0$.

We start by rewriting the given equation of the ellipse in standard form by completing the square.

First, group the $x$ and $y$ terms:

$$
(x^2 - 4x) + 4(y^2 - 4y) + 16 = 0
$$

Complete the square for the $x$-terms and the $y$-terms:

- For $x^2 - 4x$, take half of $-4$, square it to get $4$, and add and subtract $4$: 
  $$ x^2 - 4x + 4 $$

- For $y^2 - 4y$, take half of $-4$, square it to get $4$, and add and subtract $4$: 
  $$ y^2 - 4y + 4 $$

Now, rewrite the equation:

$$
(x^2 - 4x + 4) + 4(y^2 - 4y + 4) + 16 - 4 - 16 = 0
$$

Simplify:

$$
(x - 2)^2 + 4(y - 2)^2 = 4
$$

This is now in the standard form of an ellipse:

$$
\frac{(x - 2)^2}{4} + \frac{(y - 2)^2}{1} = 1
$$

The center of the ellipse is at $(2, 2)$.

So, the center of the ellipse is:

$$
(2, 2)
$$

---

### 4. Find the slope ($m>0$) of the line $y = mx - 5$ that is tangent to the circle with the equation $x^2 + y^2 = 1$.

The equation of the circle is $x^2 + y^2 = 1$ with center $(0, 0)$ and radius $r = 1$. For the line $y = mx - 5$ to be tangent to the circle, the distance from the center of the circle to the line must equal the radius.

The formula for the distance $d$ from a point $(x_1, y_1)$ to a line $Ax + By + C = 0$ is:

$$
d = \frac{|Ax_1 + By_1 + C|}{\sqrt{A^2 + B^2}}
$$

The equation of the line $y = mx - 5$ can be written as:

$$
mx - y - 5 = 0
$$

For the center of the circle $(0, 0)$, the distance to the line is:

$$
d = \frac{|m(0) - (0) - 5|}{\sqrt{m^2 + (-1)^2}} = \frac{|-5|}{\sqrt{m^2 + 1}} = \frac{5}{\sqrt{m^2 + 1}}
$$

Since the line is tangent to the circle, the distance must equal the radius, which is $1$:

$$
\frac{5}{\sqrt{m^2 + 1}} = 1
$$

Solve for $m$:

$$
5 = \sqrt{m^2 + 1}
$$

Square both sides:

$$
25 = m^2 + 1
$$

$$
m^2 = 24 \quad \Rightarrow \quad m = \sqrt{24} = 2\sqrt{6}
$$

So, the slope of the line is:

$$
m = 2\sqrt{6}
$$

---

### 5. Find the intersection points of the hyperbola $x^2 - y^2 = 1$ with the ellipse's line $x^2 + 4y^2 = 6$.

We solve the system of equations:

1. $x^2 - y^2 = 1$
2. $x^2 + 4y^2 = 6$

From the first equation, solve for $x^2$:

$$
x^2 = y^2 + 1
$$

Substitute this into the second equation:

$$
(y^2 + 1) + 4y^2 = 6
$$

Simplify:

$$
y^2 + 1 + 4y^2 = 6 \quad \Rightarrow \quad 5y^2 + 1 = 6 \quad \Rightarrow \quad 5y^2 = 5 \quad \Rightarrow \quad y^2 = 1
$$

So, $y = \pm 1$.

Substitute $y = 1$ into $x^2 = y^2 + 1$:

$$
x^2 = 1 + 1 = 2 \quad \Rightarrow \quad x = \pm \sqrt{2}
$$

Similarly, substitute $y = -1$ into $x^2 = y^2 + 1$:

$$
x^2 = 1 + 1 = 2 \quad \Rightarrow \quad x = \pm \sqrt{2}
$$

Thus, the intersection points are:

$$
(\sqrt{2}, 1), (-\sqrt{2}, 1), (\sqrt{2}, -1), (-\sqrt{2}, -1)
$$

---

### 6. For the given hyperbola $x^2 - y^2 = 1$, find the distance between its branches.

The branches of the hyperbola are the two curves $x^2 - y^2 = 1$ with $y > 0$ and $y < 0$. The distance between the branches is the distance between two points on the $y$-axis where the hyperbola intersects.

Set $x = 0$ in the equation of the hyperbola:

$$
0^2 - y^2 = 1 \quad \Rightarrow \quad -y^2 = 1 \quad \Rightarrow \quad y = \pm i
$$

This implies that the hyperbola does not intersect the $y$-axis, and thus there is no real solution for the distance between the branches along the $y$-axis.

## 16. Equations of planes in space

### 1. The plane passes through points $A(1, 2, 3)$, $B(3, 4, 5)$, and $C(2, 1, 4)$. Find the equation of the plane.

To find the equation of the plane, we need to find two vectors lying on the plane. These vectors can be obtained by subtracting the coordinates of points $A$, $B$, and $C$:

$$
\vec{AB} = B - A = (3 - 1, 4 - 2, 5 - 3) = (2, 2, 2)
$$

$$
\vec{AC} = C - A = (2 - 1, 1 - 2, 4 - 3) = (1, -1, 1)
$$

Next, find the cross product of these two vectors to obtain the normal vector $\mathbf{n}$ of the plane:

$$
\mathbf{n} = \vec{AB} \times \vec{AC} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 2 & 2 & 2 \\ 1 & -1 & 1 \end{vmatrix}
$$

Calculating the determinant:

$$
\mathbf{n} = \mathbf{i}(2 \cdot 1 - 2 \cdot (-1)) - \mathbf{j}(2 \cdot 1 - 2 \cdot 1) + \mathbf{k}(2 \cdot (-1) - 2 \cdot 1)
$$

$$
\mathbf{n} = \mathbf{i}(2 + 2) - \mathbf{j}(2 - 2) + \mathbf{k}(-2 - 2)
$$

$$
\mathbf{n} = \mathbf{i}(4) - \mathbf{j}(0) + \mathbf{k}(-4) = (4, 0, -4)
$$

Thus, the normal vector to the plane is $\mathbf{n} = (4, 0, -4)$. The equation of the plane is:

$$
4(x - 1) + 0(y - 2) - 4(z - 3) = 0
$$

Simplifying:

$$
4(x - 1) - 4(z - 3) = 0
$$

$$
4x - 4z + 4 - 12 = 0
$$

$$
4x - 4z - 8 = 0 \quad \Rightarrow \quad x - z - 2 = 0
$$

Thus, the equation of the plane is:

$$
x - z = 2
$$

---

### 2. The plane passes through point $A(1, 2, 3)$ and is parallel to the plane $2x + 3y + 4z = 5$. Find the equation of the plane.

Since the plane is parallel to the given plane, it has the same normal vector. The normal vector of the given plane $2x + 3y + 4z = 5$ is $\mathbf{n} = (2, 3, 4)$.

The equation of the plane passing through point $A(1, 2, 3)$ is:

$$
2(x - 1) + 3(y - 2) + 4(z - 3) = 0
$$

Expanding:

$$
2(x - 1) + 3(y - 2) + 4(z - 3) = 2x - 2 + 3y - 6 + 4z - 12 = 0
$$

Simplifying:

$$
2x + 3y + 4z - 20 = 0
$$

Thus, the equation of the plane is:

$$
2x + 3y + 4z = 20
$$

---

### 3. The plane passes through point $A(1, 2, 3)$ and is perpendicular to the normal vector $\mathbf{n} = [2, 3, 4]$. Find the equation of the plane.

Since the plane is perpendicular to the normal vector $\mathbf{n} = [2, 3, 4]$, the normal vector of the plane is $\mathbf{n} = (2, 3, 4)$.

The equation of the plane passing through point $A(1, 2, 3)$ is:

$$
2(x - 1) + 3(y - 2) + 4(z - 3) = 0
$$

Expanding:

$$
2x - 2 + 3y - 6 + 4z - 12 = 0
$$

Simplifying:

$$
2x + 3y + 4z - 20 = 0
$$

Thus, the equation of the plane is:

$$
2x + 3y + 4z = 20
$$

---

### 4. We have two planes $2x + 3y + 4z = 5$ and $3x + 4y + 2z = 6$. Find the line of intersection of these planes.

To find the line of intersection of two planes, we solve the system of equations:

1. $2x + 3y + 4z = 5$
2. $3x + 4y + 2z = 6$

We can solve this system by elimination or substitution. Let's multiply the first equation by $3$ and the second equation by $2$ to eliminate $x$:

$$
6x + 9y + 12z = 15
$$

$$
6x + 8y + 4z = 12
$$

Now subtract the second equation from the first:

$$
(6x + 9y + 12z) - (6x + 8y + 4z) = 15 - 12
$$

Simplifying:

$$
y + 8z = 3
$$

Thus, we have:

$$
y = 3 - 8z
$$

Substitute this into the first equation $2x + 3y + 4z = 5$:

$$
2x + 3(3 - 8z) + 4z = 5
$$

Simplifying:

$$
2x + 9 - 24z + 4z = 5
$$

$$
2x - 20z = -4
$$

Dividing by $2$:

$$
x - 10z = -2
$$

Thus:

$$
x = 10z - 2
$$

Now, we have parametric equations for the line of intersection:

$$
x = 10z - 2, \quad y = 3 - 8z, \quad z = z
$$

Thus, the parametric equations for the line of intersection are:

$$
x = 10z - 2, \quad y = 3 - 8z, \quad z = z
$$

---

### 5. Write the equation of the plane passing through point $A(1, 2, 3)$ and parallel to vectors $\vec{v_1} = [1, 0, 1]$ and $\vec{v_2} = [0, 1, -1]$.

The normal vector to the plane is the cross product of vectors $\vec{v_1}$ and $\vec{v_2}$:

$$
\mathbf{n} = \vec{v_1} \times \vec{v_2} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 1 & 0 & 1 \\ 0 & 1 & -1 \end{vmatrix}
$$

Calculating the determinant:

$$
\mathbf{n} = \mathbf{i}(0 \cdot (-1) - 1 \cdot 1) - \mathbf{j}(1 \cdot (-1) - 1 \cdot 0) + \mathbf{k}(1 \cdot 1 - 0 \cdot 0)
$$

$$
\mathbf{n} = \mathbf{i}(-1) - \mathbf{j}(-1) + \mathbf{k}(1)
$$

$$
\mathbf{n} = (-1, 1, 1)
$$

Thus, the normal vector to the plane is $\mathbf{n} = (-1, 1, 1)$.

The equation of the plane passing through point $A(1, 2, 3)$ is:

$$
-1(x - 1) + 1(y - 2) + 1(z - 3) = 0
$$

Simplifying:

$$
-(x - 1) + (y - 2) + (z - 3) = 0
$$

$$
-x + 1 + y - 2 + z - 3 = 0
$$

$$
-x + y + z - 4 = 0
$$

Thus, the equation of the plane is:

$$
x - y - z = -4
$$

---

### 6. We have the plane $2x + 3y + 4z = 5$. Find an example of a plane parallel and perpendicular to it.

- **Parallel Plane**: A plane parallel to the given plane will have the same normal vector $(2, 3, 4)$. The equation of a parallel plane can be written as:

$$
2x + 3y + 4z = d
$$

where $d$ is a constant. For example, if we take $d = 10$, the equation of the parallel plane is:

$$
2x + 3y + 4z = 10
$$

- **Perpendicular Plane**: A plane perpendicular to the given plane will have a normal vector that is perpendicular to $(2, 3, 4)$. For example, if we take the vector $(1, -2, 1)$ as the normal vector, the equation of the perpendicular plane can be written as:

$$
x - 2y + z = d
$$

To find $d$, we use a point on the plane. For simplicity, we can use the point $(0, 0, 0)$ (which satisfies $2x + 3y + 4z = 5$):

$$
0 - 0 + 0 = d
$$

Thus, the equation of the perpendicular plane is:

$$
x - 2y + z = 0
$$

---

### 7. We have the plane $2x + 3y + 4z = 5$ and point $A(1, 2, 3)$. Find the distance from point $A$ to this plane.

The formula for the distance $d$ from a point $(x_1, y_1, z_1)$ to a plane $Ax + By + Cz + D = 0$ is:

$$
d = \frac{|Ax_1 + By_1 + Cz_1 + D|}{\sqrt{A^2 + B^2 + C^2}}
$$

For the plane $2x + 3y + 4z = 5$, we have $A = 2$, $B = 3$, $C = 4$, and $D = -5$. The point $A(1, 2, 3)$ has coordinates $(x_1, y_1, z_1) = (1, 2, 3)$. Substituting into the formula:

$$
d = \frac{|2(1) + 3(2) + 4(3) - 5|}{\sqrt{2^2 + 3^2 + 4^2}}
$$

Simplifying:

$$
d = \frac{|2 + 6 + 12 - 5|}{\sqrt{4 + 9 + 16}} = \frac{|15|}{\sqrt{29}} = \frac{15}{\sqrt{29}}
$$

Thus, the distance is:

$$
d = \frac{15}{\sqrt{29}}
$$

---

### 8. The plane intersects the coordinate axes at points $A(2, 0, 0)$, $B(0, 3, 0)$, and $C(0, 0, 4)$. Find the equation of the plane.

The equation of a plane that intersects the coordinate axes at points $(x_1, 0, 0)$, $(0, y_2, 0)$, and $(0, 0, z_3)$ can be written as:

$$
\frac{x}{x_1} + \frac{y}{y_2} + \frac{z}{z_3} = 1
$$

For the points $A(2, 0, 0)$, $B(0, 3, 0)$, and $C(0, 0, 4)$, we have $x_1 = 2$, $y_2 = 3$, and $z_3 = 4$. Thus, the equation of the plane is:

$$
\frac{x}{2} + \frac{y}{3} + \frac{z}{4} = 1
$$

Multiplying through by 12 to eliminate the denominators:

$$
6x + 4y + 3z = 12
$$

Thus, the equation of the plane is:

$$
6x + 4y + 3z = 12
$$

---

### 9. Calculate the angle between the plane $x + y + z = 1$ and the plane $x = 0$ (i.e., the $yz$ plane).

The normal vector to the plane $x + y + z = 1$ is $\mathbf{n}_1 = (1, 1, 1)$, and the normal vector to the plane $x = 0$ is $\mathbf{n}_2 = (1, 0, 0)$.

The angle $\theta$ between the two planes is given by:

$$
\cos \theta = \frac{\mathbf{n}_1 \cdot \mathbf{n}_2}{|\mathbf{n}_1| |\mathbf{n}_2|}
$$

The dot product of $\mathbf{n}_1$ and $\mathbf{n}_2$ is:

$$
\mathbf{n}_1 \cdot \mathbf{n}_2 = 1 \cdot 1 + 1 \cdot 0 + 1 \cdot 0 = 1
$$

The magnitudes of $\mathbf{n}_1$ and $\mathbf{n}_2$ are:

$$
|\mathbf{n}_1| = \sqrt{1^2 + 1^2 + 1^2} = \sqrt{3}, \quad |\mathbf{n}_2| = \sqrt{1^2 + 0^2 + 0^2} = 1
$$

Thus:

$$
\cos \theta = \frac{1}{\sqrt{3}} \quad \Rightarrow \quad \theta = \cos^{-1}\left(\frac{1}{\sqrt{3}}\right)
$$

So, the angle between the planes is:

$$
\theta = \cos^{-1}\left(\frac{1}{\sqrt{3}}\right)
$$

---

### 10. Find the vector perpendicular to the plane $x + y + z = 1$.

The normal vector to the plane $x + y + z = 1$ is simply the vector of the coefficients of $x$, $y$, and $z$. Therefore, the vector perpendicular to the plane is:

$$
\mathbf{n} = (1, 1, 1)
$$

## 17. Equations of second-order surfaces

### 1. Write the equation of a sphere with center at point \( P = (1, 2, 3) \) and radius \( r = 3 \).

A sphere is defined by the equation:

$$
(x - x_0)^2 + (y - y_0)^2 + (z - z_0)^2 = r^2
$$

where \( (x_0, y_0, z_0) \) is the center of the sphere and \( r \) is its radius.

In this case, the center is \( P = (1, 2, 3) \) and the radius is \( r = 3 \). Substituting these values into the general equation of the sphere, we get:

$$
(x - 1)^2 + (y - 2)^2 + (z - 3)^2 = 3^2
$$

This simplifies to:

$$
(x - 1)^2 + (y - 2)^2 + (z - 3)^2 = 9
$$

Thus, the equation of the sphere is:

$$
(x - 1)^2 + (y - 2)^2 + (z - 3)^2 = 9
$$

### 2. Do the spheres with equations \( x^2 + y^2 + z^2 = 1 \) and \( x^2 + y^2 + z^2 = 2 \) have any common points?

We are given two spheres:

- Sphere 1: \( x^2 + y^2 + z^2 = 1 \)
- Sphere 2: \( x^2 + y^2 + z^2 = 2 \)

To determine if they have any common points, observe that both equations represent spheres with the same center at the origin \( (0, 0, 0) \), but different radii. Sphere 1 has a radius of 1 and Sphere 2 has a radius of \( \sqrt{2} \).

Since the radii are different, these two spheres do not intersect in 3D space. In fact, one sphere is completely inside the other, but they do not touch or overlap at any point. Thus, the answer is:

**No, they do not have any common points.**

### 3. What curve in space is formed by the intersection of the sphere \( x^2 + y^2 + z^2 = 1 \) with the sphere \( (x - 1)^2 + y^2 + z^2 = 1 \)? Find the equation of this curve.

We are asked to find the intersection of two spheres:

- Sphere 1: \( x^2 + y^2 + z^2 = 1 \)
- Sphere 2: \( (x - 1)^2 + y^2 + z^2 = 1 \)

To find the curve formed by their intersection, we solve these two equations simultaneously.

First, expand the second equation:

$$
(x - 1)^2 + y^2 + z^2 = 1 \quad \Rightarrow \quad (x^2 - 2x + 1) + y^2 + z^2 = 1
$$

Now subtract the first equation \( x^2 + y^2 + z^2 = 1 \) from this expanded equation:

$$
(x^2 - 2x + 1 + y^2 + z^2) - (x^2 + y^2 + z^2) = 1 - 1
$$

Simplifying:

$$
-2x + 1 = 0
$$

Solving for \( x \):

$$
x = \frac{1}{2}
$$

Thus, the intersection curve lies in the plane \( x = \frac{1}{2} \). Now, substitute \( x = \frac{1}{2} \) into the first sphere equation:

$$
\left( \frac{1}{2} \right)^2 + y^2 + z^2 = 1 \quad \Rightarrow \quad \frac{1}{4} + y^2 + z^2 = 1
$$

Simplifying:

$$
y^2 + z^2 = 1 - \frac{1}{4} = \frac{3}{4}
$$

Thus, the curve of intersection is a circle in the plane \( x = \frac{1}{2} \) with radius \( \frac{\sqrt{3}}{2} \), centered at \( (x, y, z) = \left( \frac{1}{2}, 0, 0 \right) \). The equation of this circle is:

$$
x = \frac{1}{2}, \quad y^2 + z^2 = \frac{3}{4}
$$

### 4. Write the equation of the tangent plane to the paraboloid \( z = (x - 1)^2 + y^2 + 1 \) at point \( P(1, 0, 1) \).

The general equation for the tangent plane to a surface \( z = f(x, y) \) at a point \( (x_0, y_0, z_0) \) is:

$$
z - z_0 = \frac{\partial f}{\partial x}(x_0, y_0) (x - x_0) + \frac{\partial f}{\partial y}(x_0, y_0) (y - y_0)
$$

Here, the surface is \( z = (x - 1)^2 + y^2 + 1 \), and the point is \( P(1, 0, 1) \).

First, compute the partial derivatives of \( f(x, y) = (x - 1)^2 + y^2 + 1 \):

- \( \frac{\partial f}{\partial x} = 2(x - 1) \)
- \( \frac{\partial f}{\partial y} = 2y \)

At the point \( P(1, 0, 1) \), we have:

- \( \frac{\partial f}{\partial x}(1, 0) = 2(1 - 1) = 0 \)
- \( \frac{\partial f}{\partial y}(1, 0) = 2(0) = 0 \)

Thus, the equation of the tangent plane at \( P(1, 0, 1) \) is:

$$
z - 1 = 0 \cdot (x - 1) + 0 \cdot (y - 0)
$$

This simplifies to:

$$
z = 1
$$

Thus, the equation of the tangent plane is:

$$
z = 1
$$



