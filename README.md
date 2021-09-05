# JmeterParamsDemo

Parameters from JMeter Maven Plugin
To pass parameters from Maven project using JMeter Maven plugin, 
please make sure you have Maven project created and  udated JMX placed at src/test/jmeter source folder.
If not please first setup your project Running JMeter Script from Eclipse in Maven project

Update POM.xml

Add Parameters Configuration in POM.xml
<configuration>
    <testResultsTimestamp>false</testResultsTimestamp>
    <propertiesUser>
        <threads>${threadCount}</threads>
        <rampup>${rampupTime}</rampup>
        <duration>${durationSecond}</duration>
    </propertiesUser>
</configuration>
