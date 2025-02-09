
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

---

### code to show that slope = rise over run 

```python
import matplotlib.pyplot as plt

def create_slope_chart():
    """Creates the two slope charts with explanations."""

    # Set up the figure and subplots
    fig, axs = plt.subplots(1, 2, figsize=(10, 5))
    # Data for the line
    x_vals = [-2,5]
    y_vals = [3.0, 0.5]

    # Data for triangle
    A_x = 1
    A_y = 2
    B_x = 3
    B_y = 1
    
    
    # Chart 1: Line with points A and B
    axs[0].plot(x_vals, y_vals, color='steelblue', linewidth=1.5)
    axs[0].scatter([A_x, B_x], [A_y, B_y], color='navy', s=50)
    axs[0].text(A_x - 0.2, A_y + 0.2, 'A', fontsize=12)
    axs[0].text(B_x - 0.2, B_y + 0.2, 'B', fontsize=12)
    axs[0].set_xlim(-2.5, 5.5)
    axs[0].set_ylim(-1.5, 4.5)
    axs[0].set_xticks(range(-2, 6))
    axs[0].set_yticks(range(-1, 5))
    axs[0].set_xlabel('x')
    axs[0].set_ylabel('y')
    axs[0].grid(True)
    
    # Add explanation text to the first chart
    axs[0].text(-2.4,4.2, "Pick two points:", fontsize = 10)
    axs[0].text(-2.4,3.8, "A (1, 2) and", fontsize = 10)
    axs[0].text(-2.4,3.4, "B (3, 1).", fontsize = 10)

    # Chart 2: Line with slope triangle
    axs[1].plot(x_vals, y_vals, color='steelblue', linewidth=1.5)
    axs[1].scatter([A_x, B_x], [A_y, B_y], color='navy', s=50)
    axs[1].text(A_x - 0.2, A_y + 0.2, 'A', fontsize=12)
    axs[1].text(B_x - 0.2, B_y + 0.2, 'B', fontsize=12)
    axs[1].plot([A_x, A_x], [A_y, B_y], color='orange', linestyle='-', linewidth=1.5)
    axs[1].plot([A_x, B_x], [B_y, B_y], color='orange', linestyle='-', linewidth=1.5)
    axs[1].set_xlim(-2.5, 5.5)
    axs[1].set_ylim(-1.5, 4.5)
    axs[1].set_xticks(range(-2, 6))
    axs[1].set_yticks(range(-1, 5))
    axs[1].set_xlabel('x')
    axs[1].set_ylabel('y')
    axs[1].grid(True)
    
    # Add explanation text to the second chart
    axs[1].text(-2.4,4.2, "Start with the point farthest to the left.", fontsize = 10)
    axs[1].text(-2.4,3.8, "Draw a right triangle", fontsize = 10)
    axs[1].text(-2.4,3.4, "to get from A to B.", fontsize = 10)

    axs[1].text(3.5, 1.8, 'RISE = -1', fontsize=10)
    axs[1].text(3.5, 1.5, '(Because you moved down 1 space.)', fontsize=10)
    axs[1].text(3.5, 1.2, 'RUN = 2', fontsize=10)
    axs[1].text(3.5, 0.9, '(Because you moved right 2 spaces.)', fontsize=10)

    axs[1].text(3.5, 0.5, 'SLOPE = RISE / RUN = -1 / 2', fontsize=10)
    #axs[1].text(-2.4, -1, '(The slope is -1/2 everywhere on the line.)', fontsize=10)
    #axs[1].text(-2.4, -1.3, "Any time you rise -1 and run 2, you'll be back on the line.)", fontsize=10)


    plt.tight_layout()
    plt.savefig("chart_slope_rise_over_run_example.svg", format="svg")
    plt.show()

# Run the function
create_slope_chart()
```

---
### code to generate different types of slopes 

```python
import matplotlib.pyplot as plt
import numpy as np

def plot_slope_types_subplot_with_axes():
    """
    Plots the four types of slopes (positive, negative, zero, and undefined) in a 2x2 subplot layout.
    Each subplot shows x and y ticks with all units, and the x and y axes are displayed.
    """

    # Define the range for x-values
    x = np.linspace(-5, 5, 100)

    fig, axes = plt.subplots(2, 2, figsize=(10, 8))  # Create a figure with 2x2 subplots

    # 1. Positive Slope
    y_positive = 0.5 * x
    axes[0, 0].plot(x, y_positive, color='green')
    axes[0, 0].set_title("Positive Slope")
    axes[0, 0].set_xticks(np.arange(-5, 6, 1))  # Set x-ticks at every integer value
    axes[0, 0].set_yticks(np.arange(-5, 6, 1))  # Set y-ticks at every integer value
    axes[0, 0].set_xlabel("x")
    axes[0, 0].set_ylabel("y")
    axes[0, 0].grid(True)
    axes[0, 0].axhline(0, color='black', linewidth=0.5) #add horizontal axis
    axes[0, 0].axvline(0, color='black', linewidth=0.5) #add vertical axis

    # 2. Negative Slope
    y_negative = -0.5 * x
    axes[0, 1].plot(x, y_negative, color='purple')
    axes[0, 1].set_title("Negative Slope")
    axes[0, 1].set_xticks(np.arange(-5, 6, 1))
    axes[0, 1].set_yticks(np.arange(-5, 6, 1))
    axes[0, 1].set_xlabel("x")
    axes[0, 1].set_ylabel("y")
    axes[0, 1].grid(True)
    axes[0, 1].axhline(0, color='black', linewidth=0.5) #add horizontal axis
    axes[0, 1].axvline(0, color='black', linewidth=0.5) #add vertical axis

    # 3. Zero Slope
    y_zero = np.zeros_like(x)
    axes[1, 0].plot(x, y_zero + 2 , color='blue')
    axes[1, 0].set_title("Zero Slope")
    axes[1, 0].set_xticks(np.arange(-5, 6, 1))
    axes[1, 0].set_yticks(np.arange(-5, 6, 1))
    axes[1, 0].set_xlabel("x")
    axes[1, 0].set_ylabel("y")
    axes[1, 0].grid(True)
    axes[1, 0].axhline(0, color='black', linewidth=0.5) #add horizontal axis
    axes[1, 0].axvline(0, color='black', linewidth=0.5) #add vertical axis

    # 4. Undefined Slope
    axes[1, 1].axvline(2, color='yellow')  ## the line with undefined slop 
    axes[1, 1].set_title("Undefined Slope")
    axes[1, 1].set_xticks(np.arange(-5, 6, 1))
    axes[1, 1].set_yticks(np.arange(-5, 6, 1))
    axes[1, 1].set_xlabel("x")
    axes[1, 1].set_ylabel("y")
    axes[1, 1].grid(True)
    axes[1, 1].axhline(0, color='black', linewidth=0.5) #add horizontal axis
    axes[1, 1].axvline(0, color='black', linewidth=0.5) #add vertical axis
    
    
    # Adjust layout to prevent titles/labels overlap
    plt.tight_layout()

    plt.savefig("chart_types_of_slopes.svg", format="svg")
    plt.show()
    
plot_slope_types_subplot_with_axes() 

```


---

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

---

### code to generate lines with customizable intervals 


```python
import matplotlib.pyplot as plt
import numpy as np

def plot_line(m, c, x_increment=1, y_increment=1, x_label_interval=1, y_label_interval=1, xfigure_name='chart_01.png'):
    """
    Plots a line with customizable x and y axis increments and label intervals.

    Args:
        m: Slope.
        c: Y-intercept.
        x_increment: Increment for x-axis ticks.
        y_increment: Increment for y-axis ticks.
        x_label_interval: Show x-axis labels every this many ticks.
        y_label_interval: Show y-axis labels every this many ticks.
        xfigure_name: Filename.
    """
    x_values = [-10, 10]
    y_values = [m * x + c for x in x_values]

    fig, ax = plt.subplots(figsize=(8, 8))
    ax.plot(x_values, y_values, label=f"y = {m}x + {c}", color="blue")
    ax.axhline(0, color='black', linewidth=0.8)
    ax.axvline(0, color='black', linewidth=0.8)
    ax.set_xlim(-10, 10)
    ax.set_ylim(-10, 10)
    ax.grid(color='gray', linestyle='--', linewidth=0.5)

    # --- X-Axis Ticks and Labels ---
    x_ticks = np.arange(-10, 11, x_increment)
    ax.xaxis.set_ticks(x_ticks)

    x_labels = []
    for i, x in enumerate(x_ticks):
        if i % x_label_interval == 0:  # Show label only at intervals
            x_labels.append(str(x))
        else:
            x_labels.append("")  # Empty string for no label
    ax.xaxis.set_ticklabels(x_labels, va='top')

    # --- Y-Axis Ticks and Labels ---
    y_ticks = np.arange(-10, 11, y_increment)
    ax.yaxis.set_ticks(y_ticks)

    y_labels = []
    for i, y in enumerate(y_ticks):
        if i % y_label_interval == 0:  # Show label only at intervals
            y_labels.append(str(y))
        else:
            y_labels.append("") #Empty string for no label.
    ax.yaxis.set_ticklabels(y_labels, ha='right')


    # --- Move spines ---
    ax.spines['left'].set_position('zero')
    ax.spines['bottom'].set_position('zero')
    ax.spines['right'].set_visible(False)
    ax.spines['top'].set_visible(False)

    # --- Tick parameters ---
    ax.tick_params(axis='x', which='major', direction='out', length=6, width=0.8, colors='black', top=False, bottom=False)
    ax.tick_params(axis='y', which='major', direction='out', length=6, width=0.8, colors='black', left=False, right=False)

    plt.savefig(xfigure_name)
    plt.show()
    
#plot_line(0.5, -3, x_increment=0.5, y_increment=0.5)  # X increment of 0.5, Y increment of 1    

plot_line(0,-4, x_increment=1, y_increment=1, x_label_interval=2, y_label_interval=2)


```
