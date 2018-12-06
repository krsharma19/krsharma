# Steps to write custom config management code
Open the Bussiness Works (BW) studio. Go to file and select plug-in project from the list. Provide it a suitable name e.g. **com.tibco.bwce.profile.sample** in this example.
After the project is created successfuly, right click on the src folder of the project to create a new package e.g. com.tico.bwce.profile.sample in this example and right click on this package to create a new JAVA class e.g. **CustomConfigManagement** in this example. 
Import **com.tibco.bwce.profile.resolver** package in this class and write the custom config management code here with the help of the helper class.

The helper class that is provided in the package com.tibco.bwce.profile.resolver for the users is called **ProfileResolverHelper**.
This class has two methods: 
* **getKeysForConfig()** 
* **replaceProfileValues()**

The first method **getKeysForConfig()** returns a list of type string to the calling function.
* This list consists of all the keys that are required to be fetched by the user from the custom config management server.
* These keys are fetched from the **pcf.substvar** file.
* The keys in the pcf.substvar file are set through the profile created by the user in the properties section of the BW application in the studio.

Use getKeysForConfig() method to get a list of the required keys whose corresponding values are required to be fetched from the custom config management server.
Write code for connecting to the custom config management server in the new main class (CustomConfigManagement in this sample) and fetch the values for the corresponding keys collected using the method getKeysForConfig().

The second method **replaceProfileValues()** accepts a Map of type <String, Value> 
and has a void return type.
* n
