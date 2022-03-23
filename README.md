
# Performance Testing
Today I want to share with you a new topic called **performance testing**. So first we'll try to learn, "What is performance testing?"

Performance testing is **the practice of evaluating how a system performs in terms of responsiveness and stability under a particular workload**. Performance tests are typically executed to examine speed, robustness, reliability, and application size.

### Types of performance testing for software

- [Load testing](https://www.guru99.com/load-testing-tutorial.html)
- [Stress testing](https://www.guru99.com/stress-testing-tutorial.html)
- [Spike testing](https://www.guru99.com/spike-testing.html)
- [Endurance testing](https://www.guru99.com/endurance-testing.html)
- [Scalability testing](https://www.guru99.com/scalability-testing.html)
- [Volume testing](https://www.guru99.com/volume-testing.html#:~:text=Volume%20Testing%20is%20a%20type,of%20data%20in%20the%20database.)

### Importance of performance testing
Performance Testing is done to provide stakeholders with information about their application regarding speed, stability, and scalability. More importantly, Performance Testing uncovers what needs to be improved before the product goes to market.

### Top 10 Performance Testing Tools
    1. LoadNinja 
    2. Apache JMeter
    3. WebLOAD
    4. LoadUI Pro
    5. LoadView
    6. NeoLoad
    7. LoadRunner
    8. Silk Performer
    9. AppLoader
    10. SmartMeter.io

Today I have used Apache JMeter. The **Apache JMeter™** application is open source software, a 100% pure Java application designed to load test functional behavior and measure performance.

## Steps of working procedures
First I downloaded the [Apache JMeter](https://jmeter.apache.org/)'s binary file. Then unzip the file and paste it into the ```C Drive```. For opening the file click on **jmeter.bat**```(C:\apache-jmeter-5.4.3\bin)```.

Then create a **Test Plan**. It's like a container that holds the full project. Then add **Thread group** into the **"Test Plan"**. A number of threads(users) can be defined in a Thread Group. Each thread simulates a real user requesting to the server under a test.

And then add **Request** under the **Thread Group**. The environment is almost okay. Then set ```url, path, query``` in the request file.

For visualizing results you can add multiple listeners. Now you can add **load(users)** in the thread group.

For more details, you can vist [Apache JMeter](https://jmeter.apache.org/usermanual/)'s official website.

## Alert 
Don't use GUI mode for load testing !, only for Test creation and Test debugging.
For load testing, use CLI Mode (was NON GUI):
   ```jmeter -n -t [jmx file] -l [results file] -e -o [Path to web report folder]```
####
 1.**Ajker Deal.jmx** is a file that I've created after setting all the environments in GUI mode at JMeter.

 2.**CSV File** is a folder where I stored the **result file** of the test plan in **CSV** format.
 
 3.**Report** is a folder where I stored the generated **HTML** report.
