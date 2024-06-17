# LidarEdgeDetection
This project involves edge detection  by processing lidar data using Python. It includes several functions for filtering lidar readings, arranging lists, and edge detection. 

## How to use
the API function edgedetection() takes lidar data and perform edge detection and returns yor the angle and verical distance of that edge wrt lidar position\
***readings from lidar must be list of lists***
***1- like this [[angle1,reading1],[angle2,reading2],[angle3,reading3].....]***\
***2- inf in many lidar means infinte which is beyond the range of the lidar***\
***3- here is lidar data samples***\
readings = [[0, 'inf'], [1, 'inf'], [2, 'inf'], [3, 'inf'], [4, 'inf'], [5, 'inf'], [6, 1], [7, 2], [8, 5], [9, 5], [10, 'inf'], [11, 'inf'],\
 [12, 'inf'], [13, 'inf'], [14, 'inf'], [15, 'inf'], [16, 'inf'], [17, 'inf'], [18, 'inf'], [19, 'inf'], [20, 'inf'], [21, 'inf'], [22, 'inf'],\
 [23, 'inf'], [24, 'inf'], [25, 'inf'], [26, 'inf'], [27, 'inf'], [28, 'inf'], [29, 'inf'], [30, 'inf'], [31, 'inf'], [32, 'inf'], [33, 'inf'],\
 [34, 'inf'], [35, 'inf'], [36, 'inf'], [37, 'inf'], [38, 'inf'], [39, 'inf'], [40, 'inf'], [41, 'inf'], [42, 'inf'], [43, 'inf'], [44, 'inf'],\
 [45, 'inf'], [46, 'inf'], [47, 'inf'], [48, 'inf'], [49, 'inf'], [50, 'inf'], [51, 'inf'], [52, 'inf'], [53, 'inf'], [54, 'inf'], [55, 'inf'],\
 [56, 'inf'], [57, 'inf'], [58, 'inf'], [59, 'inf'], [60, 'inf'], [61, 'inf'], [62, 'inf'], [63, 'inf'], [64, 'inf'], [65, 'inf'], [66, 'inf'],\
 [67, 'inf'], [68, 'inf'], [69, 'inf'], [70, 'inf'], [71, 'inf'], [72, 'inf'], [73, 'inf'], [74, 'inf'], [75, 'inf'], [76, 'inf'], [77, 'inf'], [78, 'inf'], \
 [79, 'inf'], [80, 'inf'], [81, 'inf'], [82, 'inf'], [83, 'inf'], [84, 'inf'], [85, 'inf'], [86, 'inf'], [87, 'inf'], [88, 'inf'], [89, 'inf'], [90, 'inf'],\
 [91, 'inf'], [92, 'inf'], [93, 'inf'], [94, 'inf'], [95, 'inf'], [96, 'inf'], [97, 'inf'], [98, 'inf'], [99, 'inf'], [100, 'inf'], [101, 'inf'], [102, 'inf'],\
 [103, 'inf'], [104, 'inf'], [105, 'inf'], [106, 'inf'], [107, 'inf'], [108, 'inf'], [109, 'inf'], [110, 'inf'], [111, 'inf'], [112, 'inf'], [113, 'inf'],\
 [114, 'inf'], [115, 'inf'], [116, 'inf'], [117, 'inf'], [118, 'inf'], [119, 'inf'], [120, 'inf'], [121, 'inf'], [122, 'inf'], [123, 'inf'], [124, 'inf'],\
 [125, 'inf'], [126, 'inf'], [127, 'inf'], [128, 1], [129, 1.1], [130, 1.2], [131, 0.9], [132, 0.9], [133, 0.98], [134, 0.1], [135, 0.2],
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



