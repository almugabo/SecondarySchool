
## illustrate pythagoras theorem

```python

import matplotlib.pyplot as plt

def draw_right_triangle(a=3, b=4,filename = 'pythagoras.svg'):
    """
    Draws a right triangle with sides:
      - a (vertical)
      - b (horizontal)
      - c (diagonal)
    and shows a small square at the right angle.
    """
    # Coordinates of the triangle’s vertices
    # A = (0, 0), B = (0, a), C = (b, 0)
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
    # The midpoint of the diagonal is (b/2, a/2)
    plt.text(b/2 + 0.2, a/2 + 0.2, r'$c$', fontsize=14)

    # Calculate the midpoint of the diagonal
    mid_x = b / 2
    mid_y = a / 2

    # Offset the text a bit along a perpendicular direction to the diagonal
    # The diagonal vector is roughly (b, -a); a perpendicular is (a, b)
    offset_scale = 0.2
    offset_x = offset_scale * a
    offset_y = offset_scale * b

    # Place the Pythagorean theorem text near the midpoint of the hypotenuse
    plt.text(mid_x + offset_x, 
             mid_y + offset_y, 
             r'$a^2 + b^2 = c^2$', 
             ha='center', 
             va='center', 
             fontsize=16)

    # Draw a small square at the right angle (origin)
    square_size = 0.2
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


