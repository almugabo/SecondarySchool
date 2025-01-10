
### plane coordinate 

```python
import matplotlib.pyplot as plt

def plot_coordinate_plane(max_x, max_y, xlabeled = True):
    """
    Plots a coordinate plane with specified maximum x and y values, and saves the plot as an SVG file.

    Parameters:
        max_x (int): The maximum value for the x-axis.
        max_y (int): The maximum value for the y-axis.
    """
    plt.figure(figsize=(8, 8))

    # Add horizontal and vertical axes
    plt.axhline(0, color='black', linewidth=0.8)
    plt.axvline(0, color='black', linewidth=0.8)

    # Set x and y limits
    plt.xlim(-max_x, max_x)
    plt.ylim(-max_y, max_y)

    # Add gridlines at each unit
    plt.xticks(range(-max_x, max_x + 1, 1), fontsize=10)
    plt.yticks(range(-max_y, max_y + 1, 1), fontsize=10)
    plt.grid(color='gray', linestyle='--', linewidth=0.5)

    if xlabeled:
        # Add axis labels
        plt.text(max_x, 0.3, 'x-axis', fontsize=12, ha='right', color='blue')
        plt.text(0.3, max_y, 'y-axis', fontsize=12, va='top', color='blue')
        # Add origin label
        plt.text(0.5, -0.5, 'origin', fontsize=12, color='red')

    # Add labels and title
    plt.title("Coordinate Plane")
    plt.xlabel("x")
    plt.ylabel("y")

    # Save the plot as an SVG file
    plt.savefig("coordinate_plane.svg", format="svg")
    plt.show()

plot_coordinate_plane(max_x = 6, max_y = 6, xlabeled = False)

```


### code to generate lines 

```python
import matplotlib.pyplot as plt

def plot_line(m, c, xfigure_name = 'chart_01.png'):
    """
    Plots a line given the slope (m) and intercept (c).
    """
    # Calculate two points for the line
    x_values = [-10, 10]
    y_values = [m * x + c for x in x_values]

    plt.figure(figsize=(8, 8))
    plt.plot(x_values, y_values, label=f"y = {m}x + {c}", color="blue")

    # Add horizontal and vertical axes
    plt.axhline(0, color='black', linewidth=0.8)
    plt.axvline(0, color='black', linewidth=0.8)

    # Set x and y limits
    plt.xlim(-10, 10)
    plt.ylim(-10, 10)

    # Add gridlines at each unit
    plt.xticks(range(-10, 11, 1))
    plt.yticks(range(-10, 11, 1))
    plt.grid(color='gray', linestyle='--', linewidth=0.5)

    # Add labels and title
    #plt.title(f"Graph of y = {m}x + {c}")
    #plt.xlabel("x")
    #plt.ylabel("y")
    #save 
    plt.savefig(xfigure_name)
    plt.show()


#plot_line(m = 2,    c = 3,   xfigure_name = 'chart_101.png')
#plot_line(m = 0.25, c= 1,    xfigure_name = 'chart_102.png')
#plot_line(m = 1/3,  c= 4,    xfigure_name = 'chart_103.png')
#plot_line(m = -2,   c= -6,   xfigure_name = 'chart_104.png')
#plot_line(m = -3/4,   c= 1,   xfigure_name = 'chart_105.png')



```
