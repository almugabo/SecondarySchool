


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

```
