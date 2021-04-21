# NLog.config
<?xml version="1.0" encoding="utf-8" ?>
<nlog xmlns="http://www.nlog-project.org/schemas/NLog.xsd"
      xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">

  <variable name="myvar" value="myvalue"/>
 
  <targets async="true">
    <target type="File" name="file" fileName="C:\Users\vicun\source\repos\NLogDemo\NLogDemo\log.txt" keepFileOpen="true"/> 
  </targets>

  <rules>   
    <logger name="*" minLevel="Debug" writeTo="file"/>  
  </rules>
</nlog>