# Calculation View with K-anonymity in SAP HANA, XS Advanced

[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/hana-xsa-calculation-view-anonymity)](https://api.reuse.software/info/github.com/SAP-samples/hana-xsa-calculation-view-anonymity)

## Description
This sample repository is the output of the following tutorial demonstrating how to create a calculation view with K-anonymity: https://developers.sap.com/tutorials/xsa-calculation-views-anonymization-k.html 

The project includes a table, sample data, configuration to load the sample data and the calculation view model with K-anonymity. 

You can find more information about K-anonymity and other methods to implement data privacy and data anonymization in the [SAP Help](https://help.sap.com/viewer/d48b808bcde547eea7f30bb101cb62b6/1.0.0.0/en-US). These features are available as of SAP HANA 2.0 SPS03.

## Requirements
This repository can be cloned into SAP Web IDE for SAP HANA on premise or SAP Web IDE Full Stack on SAP Cloud Platform.

**For on-premise**

- Minimum version of SAP HANA is 2.0 SPS03.
- SAP HANA with the Extended Application Services, advanced model (XS Advanced). Get a free instance with [the XS Advanced options for SAP HANA, express edition](https://developers.sap.com/topics/sap-hana-express.html).  SAP HANA, express edition can be used for free up to 32 GB of RAM even for productive use.
- The script server must be enabled in the tenant database. 
You can find more information in [this help document](https://help.sap.com/viewer/6b94445c94ae495c83a19646e7c3fd56/latest/en-US/bea764423908440b9237732a72dde846.html)
- The space in which you will deploy the repository must be mapped to the tenant database. 
More information [in this tutorial](https://www.sap.com/developer/tutorials/xsa-tenant-db-space.html)

**For SAP Cloud Platform**

- An productive account in SAP Cloud Platform with subaccounts in Neo and Cloud Foundry. **HDI containers included in the trial account will not work**
- SAP Web IDE Full Stack enabled
- An instance of the SAP HANA Service in Cloud Foundry with the script server enabled. The version of the database must be 2.0 SPS03 or higher. 

## Download and Installation
1.  In SAP Web IDE, right-click on the workspace and choose `Git - > Clone Repository`. 
2.  Enter the URL for the current repository. Wait until a message on the top right corner shows the clone has been successful.
3.  Right-click on the cloned project and choose `Settings`. Configure the Space (found under `Cloud Foundry` in SAP Web IDE Full Stack) to the space in which you want to deploy the application. _For example, in SAP HANA, express edition, the default space is `development`._
3.  Right-click on the `db` module and choose **Build**.

## Known Issues

**Problem:** Data preview from Web IDE fails with an error message.

**Solution**: Choose option `Open HDI container` and choose `K_ANONYMITY` under the column views.

## How to obtain support

Search for your error message in [answers.sap.com](https://answers.sap.com/index.html). If you are the first one with the problem, create a new question. Remember to include the following details so we can provide support:
- What you are doing
- The error messages
- Screenshots of the problem
- The environment you are using (Cloud or on-premise? Version?)
- Steps you have tried to solve the problem that failed

If you believe you have found a bug in the current repository, please create a bug report instead.

## License
Copyright (c) 2018 SAP SE or an SAP affiliate company. All rights reserved. This file is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE file](LICENSES/Apache-2.0.txt).
