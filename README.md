# JmeterParamsDemo

Parameters from JMeter Maven Plugin
To pass parameters from Maven project using JMeter Maven plugin, 
please make sure you have Maven project created and  udated JMX placed at src/test/jmeter source folder.
If not please first setup your project Running JMeter Script from Eclipse in Maven project

Update POM.xml

## Add Parameters Configuration in POM.xml
```javascript
<configuration>
    <testResultsTimestamp>false</testResultsTimestamp>
    <propertiesUser>
        <threads>${threadCount}</threads>
        <rampup>${rampupTime}</rampup>
        <duration>${durationSecond}</duration>
    </propertiesUser>
</configuration>
```
## Parameterize values in jmx
![Screen Shot 2021-09-04 at 10 54 16 PM](https://user-images.githubusercontent.com/87215340/132117006-5e26a209-63ea-4963-8d7d-c6838b99e437.png)

## Pass params in jenkins as below in maven template
![Screen Shot 2021-09-04 at 10 57 46 PM](https://user-images.githubusercontent.com/87215340/132117116-83977787-9b22-4806-a449-e2dc8995515b.png)
![Screen Shot 2021-09-04 at 10 59 51 PM](https://user-images.githubusercontent.com/87215340/132117142-e3703c92-d2d0-461a-a8b7-ea05dc4160cc.png)
## Results displayed in jenkins as below
![Screen Shot 2021-09-04 at 11 01 48 PM](https://user-images.githubusercontent.com/87215340/132117182-a3e72a1a-1d4c-4a56-a783-3b7ebec94305.png)

## Running from terminal
```javascript
bash-3.2$ mvn verify -DthreadCount=20 -DrampupTime=5
```
