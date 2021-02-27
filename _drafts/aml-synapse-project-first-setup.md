---
layout: post
title: AML and Azure Synapse Project Set-Up
author: Siri & Sai
---

Hey all! Welcome back to our Azure Synapse project, where we are building an end-to-end Azure Synapse Analytics workflow to predict the S&P 500 index. 

Sai is a bit more of an expert at using Synapse Analytics than I am, but like many of us I am constantly seeking to grow my skillset - so you all will be seeing my efforts to do this! 

To begin, I created a new resource group on portal.azure.com, and then within it, provisioned an Azure Synapse Analytics instance. In doing so, there are several settings that I found were important to clarify: 

![Entering workspace details](images/creating_synapse_ws.png "Synapse provisioning")

Under the Basics tab, we need to specify the subscription, resource group, which are boilerplate. We also need to specify the workspace name, the region, the name of the data lake we will be storing our training and testing datasets in. This is very important, I will find out soon! 

![Entering workspace details](images/creating_synapse_admin_pw.png "Synapse provisioning")

Now, under the Security tab, we also need to specify a SQL admin password which is also another important detail - and when I running through a tutorial of Synapse, I managed to forget. Don't do this - Azure doesn't have a great way to recover passwords or change them within a Synapse workspace so make sure to remember your password or you won't be able to create models, or edit any configurations. 

Once all of this was set up, I hit Review and Create and now had a Synapse workspace configured! Join us in the next post when we'll add the data to the the data lake. 




