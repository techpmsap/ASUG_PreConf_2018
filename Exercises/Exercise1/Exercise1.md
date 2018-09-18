<table width=100% border=>
<tr><td colspan=2><img src="images/spacer.png"></td></tr>
<tr><td colspan=2><h1>EXERCISE 1 - Create service destinations on both SAP Cloud Platform Neo and Cloud Foundry environments</h1></td></tr>
<tr><td><h3>ASUG PreConference 2018</h3></td><td><h1><img src="images/clock.png"> &nbsp;60 min</h1></td></tr>
</table>


## Description
In this exercise, you’ll learn how to 

* create a XSUAA service instance in SAP Cloud Foundry
* create a Destination service instance in SAP Cloud Foundry and import the required destination 


## Target group

* Developers
* People interested in learning the SAP Cloud Platform Application Programming Model  


## Goal

The goal of this document is to set up some required services for the next exercises.  

## Prerequisites
  
Here below are prerequisites for this exercise.

* An account on the SAP Cloud Platform: it will be provided by your instructor along with the required credentials
* The destination file you can download [here](files/ErpQueryEndpoint_CF.zip). Extract it in a proper location on your disk


## Steps

1. [Create the XSUAA and the destination services on SAP CF and check the Neo environemnt](#xsuaa-destination)



### <a name="xsuaa-destination"></a>Create the XSUAA and the destination services on SAP CF and check the Neo environemnt
In this chapter you are going to see how to create a couple of services instances(XSUAA, destination) on SAP Cloud Foundry and how to import a destination file into the destination instance.

1. Login to SAP Cloud Platform <https://account.hana.ondemand.com/cockpit#/globalaccount/8fd39023-a237-4d71-9b6a-ed9d1719d275/subaccounts> with the credentials provided by your instructor 
	![](images/01.png)

1. You will find two environments prepared for you: **ASUG** and **ASUGCF**. The first one, **ASUG**, is your SAP CP Neo environment and the other one, **ASUGCF**, is your SAP Cloud Foundry environment. Let's start with Cloud Foundry. Click on the **ASUGCF** tile  
	![](images/02.png)

1. Take note of the **API Endpoint** you find on the right side because it will be required in the next exercises when we will ask you to specify your SAP Cloud Foundry API Endpoint and click on **Spaces**  
	![](images/03.png)

1. Locate the space named **ASUGCF_DevXX** where **XX** is your **workstation ID** provided by your instructor and click on it  
	![](images/04.png)

1. Click on **Service Marketplace** and choose the **Authorization & Trust Management** tile  
	![](images/05.png)

1. Select **Instances** on the left hand side and click on the **New Instance** button to create a new instance of this XSUAA service  
	![](images/06.png)

1. Select the **application** plan and click **Next**  
	![](images/07.png)

1. Click **Next**  
	![](images/08.png)

1. Just click **Next** again  
	![](images/09.png)

1. Enter **bpr_xsuaa** as the instance name and click **Finish**  
	![](images/10.png)

1. Your XSUAA instance has been successfully created. Click on the **ASUGCF_DevXX** link on the toolbar to go back to your space  
	![](images/11.png)

1. Click again on the **Service MArketplace** to create an instance of the **destination** service  
	![](images/12.png)

1. Click on **Instances** and then on **New Instance**  
	![](images/13.png)

1. Choose the **lite** plan and click **Next**  
	![](images/14.png)

1. Click **Next**  
	![](images/15.png)

1. Don't select any application for the moment and click **Next** again  
	![](images/16.png)

1. Enter **bpr_destination** as the instance name and click **Finish**  
	![](images/17.png)

1. Your **bpr_destination** instance has been successfully created. Click on the name of this instance  
	![](images/18.png)

1. Select the **Destinations** tab on the left hand side and click on **Import Destination**  
	![](images/19.png)

1. Locate the file *ErpQueryEndpoint_CF* you extracted from the zip downloaded in the prerequisites to this exercise  
	![](images/20.png)

1. The file will be imported. Just enter the credentials provided by your instructor and click **Save**  
	![](images/21.png)

1. After saving, you can check the new destination by clicking on the button **Check Connection**  
	![](images/22.png)

1. You should get the message **Connection to "ErpQueryEndpoint"" established. Response returned: "302: Redirect"**. Click on **Close**  
	![](images/23.png)

1. Go back to your Global Account by clicking on the **TechEd2018** link on the top of the page
	![](images/24.png)

1. This time select the **ASUG** subaccount which corresponds to your **SAP Neo** environment 
	![](images/25.png)

1. Select **Connectivity -> Destinations** on the left hand side and just make sure that the **ErpQueryEndpoint** destination is correctly in place. Here we have already imported this destination since all the users will share it in the next exercises
	![](images/26.png)

1. Finally, click on **Services**, enter the text "**web**" in the search box, and click on the **SAP Web IDE Full-Stack** tile  
	![](images/27.png)

1. Click on **Go to Service**  
	![](images/28.png)

1. The **SAP Web IDE** tools is launched. Please bookmark this URL becaue it will be used in the next exercises  
	![](images/29.png)

1. Congratulations! You have successfully completed this exercise.



## Summary
This concludes the exercise. You should have learned how to create a XSUAA service instance in SAP Cloud Foundry and a Destination service instance in SAP Cloud Foundry. Please proceed with the next exercise.
