# Caculus

## Vectors

* Usually written as $\vec{a}$ or in bold **a**
* Or using start and end points $\vec{AB}=B-A$
* **Represent direction and length**
* No absolute starting position

### I. Vector Normalization

* **Magnitude(length) of a vector written as $||\vec{a}||$**
* Unit vector
  1. A vector with magnitude of 1
  2. Finding the unit vector of a vector (normalization): $\hat{a} = \frac{\vec{a}}{||\vec{a}||}$
  3. **Used to present directions doesn't care about length**

### II. Vector Multiplication

* **Dot product**
* Cross product
* Orthonormal bases and coordinate frames

### III. Dot(scalar) product

$$\vec{a}\cdot\vec{b}=||\vec{a}||\,||\vec{b}||\cos\theta$$
$$\cos\theta = \frac{\vec{a}\cdot\vec{b}}{||\vec{a}||\,||\vec{b}||}$$

* For unit Vectors
$$\cos\theta=\hat{a}\cdot\hat{b}$$
When both numbers are the unit vectors $\hat{a}$, the **cosine of the angle** between them can be quickly found using dot and cross products.

#### 1. Dot Product in Graphics

* Find angle between two vectors
  (e.g. cosine of angle between light source and surface)
* Finding projection of one vector on another

#### 2. Dot Product for projection

* $\vec{b}_\bot$:projection of $\vec{b}$ onto $\vec{a}$
  1. $\vec{b}_\bot$must be along $\vec{a}$ (or along $\hat{a}$)
     * $\vec{b}_\bot = k\hat{a}$
  2. What's its magnitude k?
     * $k=||\vec{b}_\bot|| = ||\vec{b}_\bot||\cos\theta$

### IV. Cross product

#### 1. Cross(vector) Product

$$a\times{b}=-b\times{a}$$
* Cross product is orthogonal to two initial vectors
* Direction determined by right-hand rule
* Useful in constructing coordinate systems (later)

#### 2. Cross product: Properties

$$\vec{x}\times\vec{y}=+\vec{z}$$$$\vec{y}\times\vec{x}=-\vec{z}$$$$\vec{y}\times\vec{z}=+\vec{x}$$$$\vec{z}\times\vec{y}=-\vec{x}$$$$\vec{z}\times\vec{x}=+\vec{y}$$$$\vec{x}\times\vec{z}=-\vec{y}$$
$$\vec{a}\times{b}=-\vec{b}\times\vec{a}$$$$\vec{a}\times\vec{a}=\vec{0}$$$$\vec{a}\times(\vec{b}+\vec{c})=\vec{a}\times\vec{b}+\vec{a}\times\vec{c}$$$$\vec{a}\times(k\vec{b})=k(\vec{a}\times\vec{b})$$

#### 3. Cross Product: Cartesian Formula

$$\vec{A}\times\vec{b}=\left(\begin{matrix}
    {y_a}{z_b}-{y_b}{z_a} \\
    {z_a}{x_b}-{x_a}{z_b} \\
    {x_a}{y_b}-{y_a}{x_b}
\end{matrix}\right)$$

#### 4. Cross Product in Graphics

* Determine left / right
* Determine inside / outside

### V. Orthonormal Bases / Coordinate frames

* **Important for representing points, poisitons, locations.**
* **Often many sets of coordinate systems**
    \- Global, local, world, model, parts of model (head, hands, ...)
* **Critical issue is transforming between thiese systems/bases**

## Matrices

* **Magical 2D arrays that haunt in every CS course**
* **In graphics, pervasisvely used to represent transformations**
    \- Translation, rotation, shear, scale
