
## illustrate pythagoras theorem

```python

import matplotlib.pyplot as plt

def draw_right_triangle(a=3, b=4, filename = 'pythagoras.svg'):
    """
    Draws a right triangle with sides:
      - a (vertical)
      - b (horizontal)
      - c (diagonal, computed from a and b)
    and shows a small square at the right angle.
    """
    # Coordinates of the triangle’s vertices
    # Point A = (0, 0)
    # Point B = (0, a)
    # Point C = (b, 0)
    x_coords = [0, 0, b]
    y_coords = [0, a, 0]

    plt.figure(figsize=(6, 4))

    # Fill the triangle with a color
    plt.fill(x_coords, y_coords, color='purple', alpha=0.5)

    # Draw the triangle edges
    plt.plot([0, 0], [0, a], color='black')  # vertical side
    plt.plot([0, b], [a, 0], color='black')  # diagonal side
    plt.plot([0, b], [0, 0], color='black')  # horizontal side

    # Label side 'a' (vertical)
    plt.text(-0.2, a/2, r'$a$', ha='right', va='center', fontsize=14)

    # Label side 'b' (horizontal)
    plt.text(b/2, -0.3, r'$b$', ha='center', va='top', fontsize=14)

    # Label side 'c' (diagonal)
    # A midpoint for diagonal is roughly (b/2, a/2)
    plt.text(b/2 + 0.2, a/2 + 0.2, r'$c$', fontsize=14)

    # Add the Pythagorean theorem text somewhere above the triangle
    plt.text(b/2, a + 0.5, r'$a^2 + b^2 = c^2$', 
             ha='center', va='bottom', fontsize=16)

    # Draw a small square at the right angle (origin)
    square_size = 0.2
    # Coordinates of the square in a clockwise or counter-clockwise order
    square_x = [0, square_size, square_size, 0, 0]
    square_y = [0, 0, square_size, square_size, 0]
    plt.plot(square_x, square_y, color='black')

    # Make axes equal and remove the axis lines/ticks
    plt.axis('equal')
    plt.axis('off')

   
    # Save the plot as an SVG file
    plt.savefig(filename, format="svg")
    plt.show()    
    

```


