# PCvt

python dependencies: 

* pathlib
* argparse
* numpy
* ros_numpy
* rospy

# quickly start

just type`python pcvt.py --help` for help. And some example as following:

* from `bin` to `pcd`:

  ```bash
  python pcvt.py --source bin --path bin_data_dir --dest pcd --output pcd_data_dir  
  ```

* from topic to pcd:

  ```bash
  python pcvt.py --source topic --topic /rslidar/points --dest pcd --output pcd_data_dir  
  ```

## attension

data fields in all kinds of input point cloud types will be changed to [ 'x', 'y', 'z', 'intensity'] in output.