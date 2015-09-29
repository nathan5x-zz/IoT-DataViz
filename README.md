## Internet of Things - Live Data Visualization from Sparkfun Sensors
Visualizing different data from SparkFun sensors using different Web APIs, JavaScript & CSS frameworks.
[Demo - Data Visualization](http://nathan5x.github.io/IoT-DataViz/)
---
### Description
This data visualization is about displaying data from two sensors, mainly SparkFun Soil Moisture sensor and RHT03 Temperature and Humidity sensor. There are three different data sources used in this project.

* data.sparkfun.com - publish the soil moisture data through Phant server APIs from Photon. Based on the data from data.sparkfun.com it displays the water level in a water tank with different color of the plant and bar chart of different data recorded.

* Particle Cloud Events - through Spark.publish() and Spark.subscribe() soil moisture sensor data are published in Particle Cloud. Using EventSource JavaScript API these events are subscribed (through event listeners) and soil moisture status is displayed.

* Serial Port - Using Socket.IO in NodeJS serial port data has been read and sent to line chart that displays temperature and humidity data as a stream. Upon capturing RHT03 sensor data these values are written to serial port from soilsensor.ino file.  

### Components Used
---
#### Kit
Sparkfun Photon Kit

#### Sensors
* [Soil Moisture Sensor](https://www.sparkfun.com/products/13322)
* [RHTO3 - Humidity and Temperature Sensor](https://www.sparkfun.com/products/10167)

#### LEDs
Standard Green, Red and Yellow LEDs

#### Resistors
4x 1K Ohm resistors


### Data Source
---
Spark Cloud Events - To display the status of soil moisture (wet or dry)
data.sparkfun.com - To animate the Water Tank with plant.
Serial Port - To stream Temperature and Humidity sensor data.

### Motivation
---
Inspired by number of dashboards at various places like Airport, Stock Markets, and Weather Monitoring Station.

### API Reference
---
This project is grateful to various Web APIs and JavaScript frameworks. Here are the list of references,

* [HighCharts](http://www.highcharts.com/demo/line-basic/dark-green)
 - HighCharts for rendering line charts.

* [jQuery](https://jquery.com/)
 - jQuery for all the DOM Manipulations.

* [Twitter Bootstrap](http://getbootstrap.com/)
 - Elegant CSS and JS framework for building responsive, and mobile first projects.

* [Custom Creative Bootstrap Theme](http://startbootstrap.com/template-overviews/creative/)
 - Custom Bootstrap theme.

### Contributors
---
Want to be one? Drop your GitHub username in comments. I will add you in the list. :)

### License
---
MIT License.
