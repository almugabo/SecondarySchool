

## code to plot the ant's journey 

```python
import matplotlib.pyplot as plt
import numpy as np


def plot_ant_journey(points):
    """Plots the ant's journey with arrows and markers at the end of each segment.

    Args:
        points: A list of tuples, where each tuple represents (x, y) coordinates.
    """

    x_coords = [point[0] for point in points]
    y_coords = [point[1] for point in points]

    plt.figure(figsize=(6, 6))
    plt.title("Ant's Journey")
    plt.xlabel("Horizontal Position (cm)")
    plt.ylabel("Vertical Position (cm)")
    plt.grid(True)
    plt.axhline(0, color='black', linewidth=0.5)
    plt.axvline(0, color='black', linewidth=0.5)

    # Plot each segment with an arrow and endpoint marker
    for i in range(len(points) - 1):
        x1, y1 = points[i]
        x2, y2 = points[i + 1]
        dx = x2 - x1
        dy = y2 - y1

         # Calculate the scaling factor based on dx and dy
        length = np.sqrt(dx**2+dy**2)
        arrow_length = 0.2 # length of arrow head
        head_width = 0.1 #width of arrow head
        #Calculate the dx and dy for the arrow head
        arrow_dx = dx*(length-arrow_length)/length
        arrow_dy = dy*(length-arrow_length)/length

        plt.arrow(x1, y1, arrow_dx, arrow_dy,
                  head_width=head_width,
                  head_length=arrow_length,
                  fc='blue',
                  ec='blue',
                  length_includes_head=True)

         # Add a circle at the start of the segment for better visibility
        plt.plot(x1,y1, 'o', color='blue', markersize=2)

        # Add a larger circle at the end of the segment
        plt.plot(x2, y2, 'o', color='red', markersize=5)


    # Add a label on the last point to show end point.
    plt.text(x_coords[-1] + 0.1, y_coords[-1], 'End Point')

    # Add the starting point.
    plt.text(x_coords[0] + 0.1, y_coords[0], 'Start Point')


    plt.axis('equal')
    plt.show()


# Example usage with your provided coordinates
ant_coordinates = [(0, 0), (5, 0), (5, 4), (3, 4), (3, -4)]
plot_ant_journey(ant_coordinates)

```
