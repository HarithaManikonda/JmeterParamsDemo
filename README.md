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

