Stop / Start all or only tagged Azure VMs in parallel
=====================================================

            

**DESCRIPTION**


This PowerShell Workflow Runbook connects to Azure using Managed Identity, retrieves the power status of VMs and turns off / on in parallel those that are turned on / off. You can attach a recurring schedule to this runbook to run it at a specific
 time.


**REQUIRED**


1. You have to create a managed identity for your automation account. 


2. An Action input parameter value that allows runbook to handle VMs power state. The parameter must be set to 'Stop' or 'Start'.
   

4.  An Action input parameter value for the Subscription ID of the VMs that you want to Start/Stop.


5. All the following PowerShell modules are required to run the cmdlets : Az.Accounts, Az.Resources, Az.Compute and Az.Automation.


**OPTIONAL**


3. A TagName input parameter value that allows scoping the VMs to only tagged VMs.


4. A TagValue input parameter value that allows scoping the VMs to a particular tag value.


**AUTHOR**


Bhawna Rawat


**LAST EDIT**


28-08-2023


**RELEASE NOTES**


2023-08-28 : Updated runbook with Managed Identity authentication



**RUNBOOK CONTENT**


** **

 
**

** **


** **

** 
**

        
    
TechNet gallery is retiring! This script was migrated from TechNet script center to GitHub by Microsoft Azure Automation product group. All the Script Center fields like Rating, RatingCount and DownloadCount have been carried over to Github as-is for the migrated scripts only. Note : The Script Center fields will not be applicable for the new repositories created in Github & hence those fields will not show up for new Github repositories.
