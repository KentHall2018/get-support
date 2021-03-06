---

copyright:

  years: 2015, 2020

lastupdated: "2020-01-13"

keywords: help managing cases, resolve issues managing cases, trouble working with cases, technical case, support center, help support center, resolve issues support center, help getting support, help support 

subcollection: get-support

---


{:tsSymptoms: .tsSymptoms}
{:tsCauses: .tsCauses}
{:tsResolve: .tsResolve}
{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:new_window: target="_blank"}


# Troubleshooting for getting support
{: #Supportcases}

You might encounter problems creating and managing {{site.data.keyword.Bluemix}} support cases, or general problems as you use the support center. In many cases, you can recover from these problems by following a few easy steps.
{:shortdesc}

## Why can't I create or edit support cases? 
{: #ts_service_broker}

You can't create or edit an {{site.data.keyword.Bluemix_notm}} support case, and you receive an error message that you don't have the appropriate access. 
{:shortdesc}

When you try to create a case the following error message is displayed:   
{: tsSymptoms}

`Looks like you don't have access to create cases for this account.`

General problems with accessing and managing support cases might be caused by 
not having the Identity and Access Management (IAM) access policy for the Support Center account management service. You must be assigned the editor or administrator role on the support center account management service to create cases. 
{: tsCauses}

To resolve the issue, the account owner, an administrator on the support center service, or the administrator on all account management services can assign an IAM policy on support center to manage cases. 
{: tsResolve}

If you're the account owner or an administrator of the Support Center, complete the following steps to create an access policy for working with support cases:

1. Go to **Manage** &gt; **Access (IAM)** and select **Users**.
2. Select a user name, and click **Access policies**. 
3. Click **Assign Access**. 
4. Select **Assign access to account management services**. 
5. From the **Service** menu, select **Support Center**. 
6. Select a role to define the level of access for the user. 


## Why can't I view all cases in the account?
{: #ts_viewcasedetails}

You can't view all of the cases in the account because you don't have access to view all users in the account. 
{:shortdesc}

When you try to view the support cases that are associated with the account, you can't see all open cases. 
{: tsSymptoms}

The account owner set the [user list visibility setting](/docs/iam?topic=iam-userlistview#userlistview) to restricted. When the setting is set as restricted, and you don't have an additional access policy for viewing users in the account, you don't have the required access to view all cases in the account. You can view only the users that you invited to the account, share a Cloud Foundry org membership with, or users who are in your classic infrastructure user hierarchy. 


You must be assigned an IAM policy with at least the Viewer role on the User management account management service in addition to your Support Center account management service access policy. To view your current access, go to **Manage** &gt; **Access (IAM)**, and select your name from the **Users** page. Click the **Access policies** tab, and review your assigned policies. 
{: tsCauses}

To resolve the issue, contact the account owner to request the appropriate access. 
{: tsResolve}

## Why can't I find a case that I previously created? 
{: #ts_viewarchivedcase}

You can't find your cases that you created before the migration from SoftLayer to the enhanced {{site.data.keyword.Bluemix_notm}} experience. 
{:shortdesc}

After you go to the **Manage cases** tab in the Support Center, you can't find any cases that you created before 2018 December 2. 
{: tsSymptoms}

Cases that were opened before 2018 December 2 are visible only from the **View archived cases** tab
{: tsCauses}

To view your cases, click **Support** > **Manage cases** > **View archived cases**.
{: tsResolve} 

## Why can't I create a technical support case? 
{: #ts_viewarchivedcase}

You can't create a technical support case.
{:shortdesc}

You can create cases that are related to access management, accounts, and billing and usage only. 
{: tsSymptoms}

Technical cases can be created only by accounts with advanced and premium support. If you have a Lite account, you must upgrade your account to create a technical support case. 
{: tsCauses}

To update your support plan, go to [{{site.data.keyword.Bluemix_notm}} support](https://www.ibm.com/cloud/support){: new_window} ![External link icon](../icons/launch-glyph.svg "External link icon"), and click **Contact us**. From there, you can communicate with an expert through chat, phone, or email.
{: tsResolve}

## Why can't I find help information in the Support Center for my services? 
{: #supportcenter-service}

You can't find any help information that's tailored to the services that are in your account. 
{:shortdesc}

The Support Center doesn't include recommended topics, common tasks, or FAQs that are specific to the services that you're working with. 
{: tsSymptoms}

Not all services provide personalized help information in the Support Center. 
{: tsCauses}

The Support Center is updated as help information for more services becomes available. You can explore the [{{site.data.keyword.Bluemix}} FAQ library](https://cloud.ibm.com/docs/faqs) to view FAQs for your services that aren't highlighted in the Support Center.
{: tsResolve}
