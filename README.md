# Overview
### Description
JMeter ElasticSearch Backend Listener is a JMeter plugin enabling you to send test results to an ElasticSearch engine. It is meant as an alternative live-monitoring tool to the built-in "InfluxDB" backend listener of JMeter. 

### Features

* ElasticSearch low-level REST client
  * Using the low-level client makes the plugin compatible with any ElasticSearch version
* Bulk requests
  * By making bulk requests, there are practically no impacts on the performance of the tests themselves. 
* Filters
  * Only send the samples you want by using Filters! Simply type them as follows in the appropriate field : ``filter1;filter2;filter3`` or ``sampleLabel_must_contain_this``.
* Verbose, semi-verbose, and quiet mode
  * __debug__ : Send request/response information of all requests (headers, body, etc.)
  * __info__ : Only send the request/response information of failed requests (headers, body, etc.)
  * __quiet__ : Only send the response time, bytes, and other metrics
* Use either Kibana or Grafana to vizualize your results!
  * [Click here to get a sample Grafana dashboard!](https://github.com/delirius325/jmeter-elasticsearch-backend-listener/wiki/JMeter-Generic-Dashboard) - All you need to do is import it into Grafana and change de data source!
* Continuous Integration support - [Build comparison!](https://github.com/delirius325/jmeter-elasticsearch-backend-listener/wiki/Continuous-Integration---Build-Comparison)
### Maven
```xml
<dependency>
  <groupId>io.github.delirius325</groupId>
  <artifactId>jmeter.backendlistener.elasticsearch</artifactId>
  <version>2.2.5</version>
</dependency>
```

## Contributing
Feel free to contribute by branching and making pull requests, or simply by suggesting ideas through the "Issues" tab.

## Screenshots
### Configuration
![screnshot1](https://cdn-images-1.medium.com/max/2000/1*iVb7mIp2dPg7zE4Ph3PrGQ.png "Screenshot of configuration")

### Sample Grafana dashboard
![screnshot1](https://image.ibb.co/jW6LNx/Screen_Shot_2018_03_21_at_10_21_18_AM.png "Sample Grafana Dashboard")

### For more info
For more information, here's a little (https://github.com/delirius325/jmeter-elasticsearch-backend-listener/wiki)[documentation].
