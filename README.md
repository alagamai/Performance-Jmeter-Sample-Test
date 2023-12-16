# Generate jmeter report using azure devops pipeline  

# Screenshots

![jmeter-report1](https://github.com/alagamai/Performance-Jmeter-Sample-Test/blob/master/images/image1.png 'jmeter-report1')
![jmeter-report2](https://github.com/alagamai/Performance-Jmeter-Sample-Test/blob/master/images/image2.png 'jmeter-report2')
![jmeter-report3](https://github.com/alagamai/Performance-Jmeter-Sample-Test/blob/master/images/image3.png 'jmeter-report3')
![jmeter-report4](https://github.com/alagamai/Performance-Jmeter-Sample-Test/blob/master/images/image4.png 'jmeter-report4')


how to run jmeter in azure devops pipeline and view reports
1. create a new pipleine 
2. install plugins - Run Perf Analyzer, Publish Html Report, publish pipeline artifact
3. in Run Perf Analyzer set JMeter Log Folder Name = CurrentLog
  and JMeter Report Folder Name = CurrentReport
4. in publish html report select htmltype as Jmeter
   and set JmeterReportsPath = $(Pipeline.Workspace)\s\apache-jmeter-5.5\bin\CurrentReport
