# LidarEdgeDetection
This project involves edge detection  by processing lidar data using Python. It includes several functions for filtering lidar readings, arranging lists, and edge detection. 

## How to use
the API function edgedetection() takes lidar data and perform edge detection and returns yor the angle and verical distance of that edge wrt lidar position\
***readings from lidar must be list of lists***
***like this [[angle1,reading1],[angle2,reading2],[angle3,reading3].....]***
***inf in many lidar means infinte which is beyond the range of the lidar***
***here is lidar data samples***
### Functions
#### `edgeDetection(readings)`
- **Description:** Performs edge detection on lidar readings.
- **Arguments:**
  - `readings` (list): List of lidar readings.
- **Returns:** 
  - `list`: List containing the results of edge detection.
  - 
#### `arrange_list(lst, order)`
- **Description:** Arranges a list into quarters based on a given order.
- **Arguments:**
  - `lst` (list): The list to be arranged.
  - `order` (str): The order specifying how the list should be arranged.
- **Returns:** 
  - `list`: The arranged list.

#### `filter_readings(readings, car_width_half=0.75)`
- **Description:** Filters lidar readings based on a given car width.
- **Arguments:**
  - `readings` (list): List of lidar readings.
  - `car_width_half` (float, optional): Half of the car's width. Defaults to 0.75.
- **Returns:** 
  - `list`: Filtered list of readings.

#### `group_lists(data, threshold=1)`
- **Description:** Groups relevant lines together based on a threshold.
- **Arguments:**
  - `data` (list): List of data points.
  - `threshold` (int, optional): Grouping threshold. Defaults to 1.
- **Returns:** 
  - `list`: Grouped list of data points.

#### `find_lowest_average(data)`
- **Description:** Calculates the lowest average from a list of data points.
- **Arguments:**
  - `data` (list): List of data points.
- **Returns:** 
  - `list`: List containing the lowest average.



