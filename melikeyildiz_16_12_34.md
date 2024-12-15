## 15. Equations of Second-order Curves (Conic Sections)

### 1. Find the equation of a circle with center at point $$A(1, 2)$$ and radius $$r = 3$$.

The general equation of a circle is:
$$
(x - h)^2 + (y - k)^2 = r^2
$$
where $$(h, k)$$ is the center and $$r$$ is the radius.

**Substitute the values:**
- Center: $$(h, k) = (1, 2)$$
- Radius: $$r = 3$$

The equation becomes:
$$
(x - 1)^2 + (y - 2)^2 = 3^2
$$
Simplify:
$$
(x - 1)^2 + (y - 2)^2 = 9
$$

### 2. Find the equation of a parabola intersecting the $$Ox$$ axis at points $$x = 2, x = 4$$, and passing through point $$y(3) = 1$$.

The general form of a parabola that opens vertically is:
$$
y = a(x - x_1)(x - x_2)
$$
where $$(x_1, 0)$$ and $$(x_2, 0)$$ are the x-intercepts.

**Substitute the given intercepts:**
- x_1 = 2$$, $$x_2 = 4
$$
y = a(x - 2)(x - 4)
$$

**Use the point $$(3, 1)$$ to find $$a$$:**
$$
1 = a(3 - 2)(3 - 4)
$$
Simplify:
$$
1 = a(1)(-1) \implies a = -1
$$

Thus, the equation of the parabola is:
$$
y = -(x - 2)(x - 4)
$$
Simplify:
$$
y = -(x^2 - 6x + 8) \implies y = -x^2 + 6x - 8
$$

### 3. Find the center of the ellipse with the equation:
$$
x^2 + 4y^2 - 4x - 16y + 16 = 0
$$

Rearrange the equation to group $$x$$ and $$y$$ terms:
$$
(x^2 - 4x) + (4y^2 - 16y) = -16
$$

Complete the square for both groups:
1. For $$x^2 - 4x$$:
   $$x^2 - 4x = (x - 2)^2 - 4$$
2. For $$4y^2 - 16y$$:
   Factor out $$4$$:
   $$4(y^2 - 4y)$$
   Complete the square inside the parentheses:
   $$y^2 - 4y = (y - 2)^2 - 4$$
   So:
   $$4(y^2 - 4y) = 4((y - 2)^2 - 4) = 4(y - 2)^2 - 16$$

Substitute back:
$$
(x - 2)^2 - 4 + 4(y - 2)^2 - 16 = -16
$$
Simplify:
$$
(x - 2)^2 + 4(y - 2)^2 = 4
$$

The center of the ellipse is:
$$
(2, 2)
$$

### 4. Find the slope $$(m > 0)$$ of the line $$y = mx - 5$$ that is tangent to the circle with the equation:
$$
x^2 + y^2 = 1
$$

The condition for tangency is that the distance from the center of the circle $$(0, 0)$$ to the line must equal the radius of the circle.

The distance from $$(0, 0)$$ to the line $$y = mx - 5$$ is given by:
$$
\text{Distance} = \frac{|c|}{\sqrt{1 + m^2}}
$$
where the line is written as $$y = mx + c$$.

Here, $$c = -5$$ and the radius is $$1$$:
$$
\frac{|-5|}{\sqrt{1 + m^2}} = 1
$$
Solve for $$m$$:
$$
\frac{5}{\sqrt{1 + m^2}} = 1 \implies 5 = \sqrt{1 + m^2}
$$
Square both sides:
$$
25 = 1 + m^2 \implies m^2 = 24
$$
Take the positive square root (since $$m > 0$$):
$$
m = \sqrt{24} = 2\sqrt{6}
$$

### 5. Find the intersection points of the hyperbola $$x^2 - y^2 = 1$$ with the ellipse's line $$x^2 + 4y^2 = 6$$.

Solve the two equations simultaneously:
1. $$x^2 - y^2 = 1$$
2. $$x^2 + 4y^2 = 6$$

**Subtract the first equation from the second:**
$$
(x^2 + 4y^2) - (x^2 - y^2) = 6 - 1
$$
Simplify:
$$
5y^2 = 5 \implies y^2 = 1 \implies y = \pm 1
$$

**Substitute $$y = 1$$ and $$y = -1$$ into the first equation:**
1. For $$y = 1$$:
   $$x^2 - (1)^2 = 1 \implies x^2 = 2 \implies x = \pm \sqrt{2}$$
2. For $$y = -1$$:
   $$x^2 - (-1)^2 = 1 \implies x^2 = 2 \implies x = \pm \sqrt{2}$$

**Intersection points:**
$$(\sqrt{2}, 1), (-\sqrt{2}, 1), (\sqrt{2}, -1), (-\sqrt{2}, -1)$$

### 6. For the given hyperbola $$x^2 - y^2 = 1$$, find the distance between its branches.

The distance between the branches of a hyperbola is defined as the distance between the two asymptotes at a given $$y$$ level. For the hyperbola $$x^2 - y^2 = 1$$, the asymptotes are:
$$
y = \pm x
$$

The horizontal distance between these lines at a given $$y$$ is:
$$
\Delta x = 2|y|
$$

Since the question asks for the distance between the branches, we use $$y = 0$$ (the closest point), and the distance is:
$$
\Delta x = 2(1) = 2
$$

## 16. Equations of Planes in Space

### 1. The plane passes through points $$A(1, 2, 3)$$, $$B(3, 4, 5)$$, and $$C(2, 1, 4)$$. Find the equation of the plane.

To find the equation of a plane, we need a point on the plane and a normal vector.

1. Compute two vectors on the plane:
   $$\vec{AB} = B - A = (3 - 1, 4 - 2, 5 - 3) = (2, 2, 2)$$
   $$\vec{AC} = C - A = (2 - 1, 1 - 2, 4 - 3) = (1, -1, 1)$$

2. Find the normal vector by taking the cross product:
   $$\vec{n} = \vec{AB} \times \vec{AC}$$
   $$\vec{n} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 2 & 2 & 2 \\ 1 & -1 & 1 \end{vmatrix}$$
   Expand:
   $$\vec{n} = \mathbf{i}(2 \times 1 - 2 \times -1) - \mathbf{j}(2 \times 1 - 2 \times 1) + \mathbf{k}(2 \times -1 - 2 \times 1)$$
   $$\vec{n} = \mathbf{i}(2 + 2) - \mathbf{j}(2 - 2) + \mathbf{k}(-2 - 2)$$
   $$\vec{n} = 4\mathbf{i} - 0\mathbf{j} - 4\mathbf{k} = (4, 0, -4)$$

3. Use the point-normal form of the plane:
   $$4(x - 1) + 0(y - 2) - 4(z - 3) = 0$$
   Simplify:
   $$4x - 4z = -8 \implies x - z = -2$$

The equation of the plane is:
$$x - z = -2$$

### 2. The plane passes through point $$A(1, 2, 3)$$ and is parallel to the plane $$2x + 3y + 4z = 5$$. Find the equation of the plane.

Planes that are parallel have the same normal vector. The normal vector of the given plane is:
$$\vec{n} = (2, 3, 4)$$

Use the point-normal form of the plane with $$\vec{n} = (2, 3, 4)$$ and point $$A(1, 2, 3)$$:
$$2(x - 1) + 3(y - 2) + 4(z - 3) = 0$$
Simplify:
$$2x - 2 + 3y - 6 + 4z - 12 = 0$$
$$2x + 3y + 4z - 20 = 0$$

The equation of the plane is:
$$2x + 3y + 4z = 20$$

### 3. The plane passes through point $$A(1, 2, 3)$$ and is perpendicular to the normal vector $$\vec{n} = [2, 3, 4]$$. Find the equation of the plane.

Use the point-normal form of the plane:
$$2(x - 1) + 3(y - 2) + 4(z - 3) = 0$$
Simplify:
$$2x - 2 + 3y - 6 + 4z - 12 = 0$$
$$2x + 3y + 4z - 20 = 0$$

The equation of the plane is:
$$2x + 3y + 4z = 20$$

### 4. We have two planes $$2x + 3y + 4z = 5$$ and $$3x + 1y + 2z = 6$$. Find the line of intersection of these planes.

To find the line of intersection, we solve the two plane equations simultaneously.

1. Parameterize one variable (e.g., $$z = t$$):
   From $$2x + 3y + 4z = 5$$:
   $$2x + 3y + 4t = 5 \implies x = \frac{5 - 3y - 4t}{2}$$

2. Substitute into the second plane equation $$3x + y + 2z = 6$$:
   $$3\left(\frac{5 - 3y - 4t}{2}\right) + y + 2t = 6$$
   Simplify:
   $$\frac{15 - 9y - 12t}{2} + y + 2t = 6$$
   Multiply through by 2 to eliminate the fraction:
   $$15 - 9y - 12t + 2y + 4t = 12$$
   $$-7y - 8t = -3 \implies y = \frac{-3 + 8t}{7}$$

3. Substitute $$y = \frac{-3 + 8t}{7}$$ and $$z = t$$ into $$x = \frac{5 - 3y - 4t}{2}$$:
   $$x = \frac{5 - 3\left(\frac{-3 + 8t}{7}\right) - 4t}{2}$$
   Simplify:
   $$x = \frac{5 - \frac{-9 + 24t}{7} - 4t}{2} = \frac{\frac{35 + 9 - 24t - 28t}{7}}{2}$$
   $$x = \frac{44 - 52t}{14} = \frac{22 - 26t}{7}$$

The parametric equations for the line of intersection are:
$$
\begin{aligned}
  x &= \frac{22 - 26t}{7} \\
  y &= \frac{-3 + 8t}{7} \\
  z &= t
\end{aligned}
$$

### 5. Write the equation of the plane passing through point $$A(1, 2, 3)$$ and parallel to vectors $$\vec{v_1} = (1, 0, 1)$$ and $$\vec{v_2} = (0, 1, -1)$$.

The normal vector $$\vec{n}$$ is the cross product of $$\vec{v_1}$$ and $$\vec{v_2}$$:
$$\vec{n} = \vec{v_1} \times \vec{v_2} = \begin{vmatrix} \mathbf{i} & \mathbf{j} & \mathbf{k} \\ 1 & 0 & 1 \\ 0 & 1 & -1 \end{vmatrix}$$
Expand:
$$\vec{n} = \mathbf{i}(0 \times -1 - 1 \times 1) - \mathbf{j}(1 \times -1 - 0 \times 0) + \mathbf{k}(1 \times 1 - 0 \times 0)$$
$$\vec{n} = \mathbf{i}(-1) - \mathbf{j}(-1) + \mathbf{k}(1)$$
$$\vec{n} = (-1, 1, 1)$$

Use the point-normal form:
$$-1(x - 1) + 1(y - 2) + 1(z - 3) = 0$$
Simplify:
$$-x + y + z = 4$$

The equation of the plane is:
$$-x + y + z = 4$$

## 17. Equations of Second-Order Surfaces

### 1. Write the equation of a sphere with center at point $$P(1, 2, 3)$$ and radius $$r = 3$$.

The equation of a sphere is given by:
$$
(x - x_0)^2 + (y - y_0)^2 + (z - z_0)^2 = r^2
$$
where $$(x_0, y_0, z_0)$$ is the center and $$r$$ is the radius.

Substitute $$P(1, 2, 3)$$ and $$r = 3$$:
$$
(x - 1)^2 + (y - 2)^2 + (z - 3)^2 = 3^2
$$
Simplify:
$$
(x - 1)^2 + (y - 2)^2 + (z - 3)^2 = 9
$$

### 2. Do the spheres with equations $$x^2 + y^2 + z^2 = 1$$ and $$x^2 + y^2 + z^2 = 2$$ have any common points?

For two spheres to have common points, their equations must be satisfied simultaneously. Consider:
$$
S_1: x^2 + y^2 + z^2 = 1
$$
$$
S_2: x^2 + y^2 + z^2 = 2
$$

The left-hand sides of both equations are identical, but the right-hand sides differ. This is a contradiction:
$$1 \neq 2$$

Thus, the two spheres have no common points.

### 3. What curve in space is formed by the intersection of the sphere $$x^2 + y^2 + z^2 = 1$$ with the sphere $$(x - 1)^2 + y^2 + z^2 = 1$$? Find the equation of this curve.

To find the curve of intersection, subtract the equations of the two spheres:
$$
(x - 1)^2 + y^2 + z^2 - (x^2 + y^2 + z^2) = 1 - 1
$$
Simplify:
$$
x^2 - 2x + 1 + y^2 + z^2 - x^2 - y^2 - z^2 = 0
$$
$$
-2x + 1 = 0
$$
Solve for $$x$$:
$$
 x = \frac{1}{2}
$$

Substitute $$x = \frac{1}{2}$$ into the equation of one of the spheres, e.g., $$x^2 + y^2 + z^2 = 1$$:
$$
\left(\frac{1}{2}\right)^2 + y^2 + z^2 = 1
$$
Simplify:
$$
\frac{1}{4} + y^2 + z^2 = 1
$$
$$
y^2 + z^2 = \frac{3}{4}
$$

The curve of intersection is a circle in the plane $$x = \frac{1}{2}$$ with the equation:
$$
y^2 + z^2 = \frac{3}{4}
$$

### 4. Write the equation of the tangent plane to the paraboloid $$z = (x - 1)^2 + y^2 + 1$$ at point $$P(1, 0, 1)$$.

The general equation of the paraboloid is:
$$
z = (x - 1)^2 + y^2 + 1
$$

1. Compute the partial derivatives:
   $$\frac{\partial z}{\partial x} = 2(x - 1)$$
   $$\frac{\partial z}{\partial y} = 2y$$

2. Evaluate the derivatives at point $$P(1, 0, 1)$$:
   $$\frac{\partial z}{\partial x} \Big|_{(1, 0, 1)} = 2(1 - 1) = 0$$
   $$\frac{\partial z}{\partial y} \Big|_{(1, 0, 1)} = 2(0) = 0$$

3. The tangent plane at $$P(x_0, y_0, z_0)$$ is given by:
   $$z - z_0 = \frac{\partial z}{\partial x}(x - x_0) + \frac{\partial z}{\partial y}(y - y_0)$$

   Substitute $$x_0 = 1$$, $$y_0 = 0$$, $$z_0 = 1$$, and the partial derivatives:
   $$z - 1 = 0 \cdot (x - 1) + 0 \cdot (y - 0)$$
   $$z = 1$$

The equation of the tangent plane is:
$$
z = 1
$$
