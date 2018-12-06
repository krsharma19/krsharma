# Steps to write custom config management code
Open the Bussiness Works (BW) studio. Go to file and select plug-in project from the list. Provide it a suitable name e.g. **com.tibco.bwce.profile.sample** in this example.
After the project is created successfuly, right click on the src folder of the project to create a new package e.g. com.tico.bwce.profile.sample in this example and right click on this package to create a new JAVA class e.g **CustomConfigManagement** in this example. 
Import **com.tibco.bwce.profile.resolver** package in this class and write the custom config management code here.

The helper class that is provided in the package com.tibco.bwce.profile.resolver for the users is called **ProfileResolverHelper**.
This class has two methods: 
* **getKeysForConfig()** 
* **replaceProfileValues()**
