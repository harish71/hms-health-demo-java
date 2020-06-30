# Health kit demo

## Table of Contents

 * [Introduction](#Introduction)
 * [Getting Started](#Getting Started)
 * [Supported Environments](#Supported Environments)
 * [Result](#Result)
 * [License](#License)


## Introduction
HUAWEI Health is an open service for sports & health capabilities provided by Huawei. Developers can access the Huawei Health Platform and obtain sports & health data by integrating HUAWEI Health.   
Health demo code encapsulates APIs of the HUAWEI Health Kit. It provides demo programs for your reference or usage.   

The following describes the functions of Health Kit:  
1)  Login and Authorization  
This function applies to login the account and enable the authorization.  
Code location:  \app\src\main\java\com\huawei\demo\hihealth\HihealthKitMainActivity.java   

2)  Operate health and sport data  
The function has ability to add/delete/update/query the health and sport data.  
Code location: \app\src\main\java\com\huawei\demo\hihealth\HihealthKitDataManagerActivity.java   
    
3) Real time update  
This function applies to update the real time data from sensors to the application layer.  
Code location:  \app\src\main\java\com\huawei\demo\hihealth\HiHealthKitSensorsControllerActivity.java   
4) Auto-record the health data  
This function can enable and disable the automatically record method for the health data.  
Code location: \app\src\main\java\com\huawei\demo\hihealth\HiHealthKitAutoRecorderControllerActivity.java   
    
5) Operate Activity Record   
This function can create and manage a single sport or activity.  
Code location:  \app\src\main\java\com\huawei\demo\hihealth\HihealthKitActivityRecordControllerActivity.java   
    
6) Operate DataType and Records  
This function can add/read DataType and cancel All Records.   
Code location:  \app\src\main\java\com\huawei\demo\hihealth\HihealthKitSettingControllerActivity.java   


## Getting Started

Before using Health demo code, check whether the IDE environment has been installed. 
1. Decompress the demo code package.    
2. Copy the Health package into the IDE directory and import it into the IDE Tool.
3. Press Sync Project with Gradle Files to ensure the development environment builds completed.

To use functions provided by packages in examples, you need to set parameters as following:
1. HuaweiAccount: Health need verify the user's permission to operate user's health data
2. HMS SDK maven Address:
    * Configure the maven address of the HMS SDK in allprojects-> repositories of project's build.gradle : maven {url 'http://developer.huawei.com/repo/'}
    * Add maven configuration of HMS SDK in buildscript-> dependencies : maven {url 'http://developer.huawei.com/repo/'}
3. Compile dependencies: Add compile dependencies in model's build.gradle : implementation 'com.huawei.hms:hihealth-base:{version}'
4. AppId info: In the application AndroidManifest.xml, add the appId information generated by the Developer Alliance when creating the application


## Supported Environments
* Android Studio 3.0 or later
* Java SDK 1.8 or later
* HMS Core 4.0.4.207 or later

## Result
   <img src="images/result_1.png" width = 30% height = 30%>
   <img src="images/result_2.png" width = 30% height = 30%>
   <img src="images/result_3.png" width = 30% height = 30%>
   <img src="images/result_4.png" width = 30% height = 30%>
   <img src="images/result_5.png" width = 30% height = 30%>
   <img src="images/result_6.png" width = 30% height = 30%>
	
##  License
   Health kit demo is licensed under the [Apache License, version 2.0](http://www.apache.org/licenses/LICENSE-2.0).