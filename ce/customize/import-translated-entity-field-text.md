---
title: "Import translated entity and field text with PowerApps | MicrosoftDocs"
description: "Learn how to import translated entity and field text"
ms.custom: ""
ms.date: 04/10/2018
ms.reviewer: ""
ms.service: "crm-online"
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "article"
applies_to: 
  - "Dynamics 365 (online)"
  - "Dynamics 365 Version 9.x"
  - "powerapps"
author: "Mattp123"
ms.assetid: 3d77d149-819b-45e6-8e70-1fbe54d5c153
caps.latest.revision: 19
ms.author: "matp"
manager: "kvivek"
search.audienceType: 
  - customizer
search.app: 
  - D365CE
---
# Import translated entity and field text back into an app

[!INCLUDE [cc-applies-to-powerapps-and-update-9-0-0](../includes/cc-applies-to-powerapps-and-update-9-0-0.md)]<br/>[!INCLUDE [cc_applies_to_on-prem-9_0_0](../includes/cc_applies_to_on-prem-9_0_0.md)]

If you have customized entity or field text, such as field labels or drop-down list values, you can provide the users in your organization who are not working with the base language version of your environment with this customized text in their own languages. To do so, you export the text strings for all your customizations so that they can be translated into the languages you use in your organization.  
  
 After the translation, you need to import the translated text strings into your environment before users can take advantage of the changes.  
  
> [!IMPORTANT]
> - The file that you import must be a compressed file that contains the CrmTranslations.xml and the [Content_Types].xml file at the root.  
> - You can’t import translated text that is over 500 characters long. If any of the items in your translation file are longer than 500 characters, the import process will fail. If the import process fails, review the line in the file that caused the failure, reduce the number of characters, and try to import again. Also note that after you import translated text, you must republish customizations.  
  
1. [!INCLUDE[proc_permissions_system_admin_and_customizer](../includes/proc-permissions-system-admin-and-customizer.md)]  
  
2. In the solution explorer, on the Actions toolbar, select **Import Translations**.  
  
3. In the **Import Translated Text** dialog box, specify the file that contains the translated text, and then select **Import**.  
  
4. When the import is complete, select **Close**.  
  
> [!NOTE]
>  Publishing customizations can interfere with normal system operation. We recommend you schedule publishing when it’s least disruptive to users.  

## Community tools

[Easy Translator](https://www.xrmtoolbox.com/plugins/MsCrmTools.Translator/) is a tool that XrmToolBox community developed for [!INCLUDE[pn_dynamics_crm](../includes/pn-dynamics-crm.md)] Customer Engagement. Use Easy Translator to export and import translations with contextual information. 

> [!NOTE]
> The community tools are not supported by [!include[pn_microsoft_dynamics](../includes/pn-microsoft-dynamics.md)]. 
> If you have questions about the tool, please contact the publisher. More Information: [XrmToolBox](https://www.xrmtoolbox.com).

### See also  
 [Export customized entity and field text for translation](../customize/export-customized-entity-field-text-translation.md)
