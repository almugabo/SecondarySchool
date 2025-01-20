

```python

import random
import matplotlib.pyplot as plt

def generate_rectangle_question():
    # Randomize dimensions
    length = random.randint(5, 15)
    width = random.randint(3, 10)
    perimeter = 2 * (length + width)
    
    # Print the question
    print(f"The lengths of the sides of the given rectangle are (x + {length}) and 2x + {width}.")
    print(f"If the perimeter is {perimeter} cm, form an equation and solve it to find the value of x.")
    
    # Draw the rectangle
    plt.figure()
    plt.plot([0, length, length, 0, 0], [0, 0, width, width, 0], 'b-', linewidth=2)
    plt.text(length / 2, -0.5, f"x + {length}", ha="center", va="top")
    plt.text(-0.5, width / 2, f"2x + {width}", ha="right", va="center", rotation="vertical")
    plt.text(length / 2, width + 0.5, f"x + {length}", ha="center", va="bottom")
    plt.text(length + 0.5, width / 2, f"2x + {width}", ha="left", va="center", rotation="vertical")
    plt.axis('off')  # Turn off the frame
    plt.show()

def generate_triangle_question():
    # Randomize dimensions
    side1 = random.randint(4, 10)
    side2 = random.randint(4, 10)
    side3 = side1 + side2 - random.randint(1, 3)  # Ensure triangle inequality holds
    perimeter = side1 + side2 + side3
    
    # Print the question
    print(f"The lengths of the sides of the given triangle are x, x - {side1}, and x - {side2}.")
    print(f"If the perimeter is {perimeter} cm, form an equation and solve it to find the value of x.")
    
    # Draw the triangle
    plt.figure()
    # Coordinates for a simple triangle
    plt.plot([0, 1, 2, 0], [0, 2, 0, 0], 'g-', linewidth=2)
    plt.text(0.5, 1.2, f"x - {side1}", ha="center", va="center")
    plt.text(1.5, 1.2, f"x - {side2}", ha="center", va="center")
    plt.text(1, -0.5, "x", ha="center", va="center")
    plt.axis('off')  # Turn off the frame
    plt.show()

# Example usage:
generate_rectangle_question()
generate_triangle_question()


```
