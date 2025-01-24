## code to generate charts 


```python

import matplotlib.pyplot as plt

def generate_distance_time_graph(points, 
                                 time_increment=20, 
                                 distance_increment=20, 
                                 units_time = 'minutes',
                                 units_distance = 'kms',
                                 graph_name = 'chart.svg',
                                ):
    """
    Generates a distance-time graph using matplotlib with customizable axis increments,
    ensuring that the origin (0,0) is at the very beginning of the chart.

    Args:
        points: A list of tuples, where each tuple represents (time, distance) coordinates.
        time_increment: The increment value for the time axis (x-axis).
        distance_increment: The increment value for the distance axis (y-axis).
    """

    # Separate the points into times and distances
    times = [point[0] for point in points]
    distances = [point[1] for point in points]

    plt.figure(figsize=(8, 6))
    plt.plot(times, distances, marker='o', linestyle='-')
    plt.xlabel('Time (time_unit)'.replace('time_unit', units_time ))
    plt.ylabel('Distance (dist_unit)'.replace('dist_unit', units_distance))
    plt.title('Distance-Time Graph')
    plt.grid(True)

    # Determine the maximum values for setting axis limits
    max_time = max(times)
    max_distance = max(distances)

    # Set the ticks for both axes starting from 0
    plt.xticks(range(0, max_time + time_increment, time_increment))
    plt.yticks(range(0, max_distance + distance_increment, distance_increment))

    # Explicitly set the axis limits to start at 0
    plt.xlim(left=0)
    plt.ylim(bottom=0)

    plt.savefig(graph_name, format="svg")
    plt.show()


``

