# SatellitePosition项目
此项目是关于学习卫星导航定位算法，并使用PY实现卫星定位算法。
目前已实现：
- 将rinex格式数据进行读取。
- 基于测码伪距的单点定位算法。
- 基于EKF的rtk相对定位算法（float解）。


## Py_study目录：
主要是关于py的一些学习，功能实现的方式等。  

## positon目录：
学习并实现卫星的定位算法

### 1、common目录：
- \_\_init\_\_：初始化类
- CoordinateTransformation.py：XYZ坐标系与BLH坐标系互相转换的功能类。  
- NAVDATA.py：包含将rinex格式的星历文件进行提取转换的方法，并打包成星历类。  
- OBSDATA.py：包含将rinex格式的观测量文件进行提取转换的方法，并打包成观测值类。
- OPTION.py：包含了一些参数配置。
- RTKCOMMON.py：包含定位算法需要用到的公共方法。
- SATPOS.py：用于计算卫星坐标的方法。
- solution.py：包含定位结果、历元时间、解算卫星数、定位状态、age等信息。
- tool.py：包含了一些常用的常参、数学方法等工具。



### 2、singlepoint目录
- \_\_init\_\_：初始化类
- singlepoint.py：主函数。  
- SINGLEPOINTPOSITION.py：实现基于测码伪距的单点定位算法。 
### 3、rtkpoint目录
- \_\_init\_\_：初始化类
- rtkpoint.py：主函数。
- RTKPOSITION.py：已实现基于EKF的相对定位算法（float解），利用了双差进行计算。

