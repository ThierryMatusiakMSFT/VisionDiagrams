# Data Lifecycle Management & Records Management

Data Lifecycle Management (DLM) protects important data during its retention period.  
It can also erase old data. 

Records Management extends DLM to prevent records updates or deletion.

## Context
Both Records Management and Data Lifecycle Management apply to M365 Data.  
Data Lifecycle Managers define a set of Retention Labels and Retention Policies.  
These policies include a data retention period (in case a user deletes this content).  
They can also result into documents' deletion after a specific period. This deletion can be automatic or go through a disposition review.  

M365 uses dedicated storage locations to preserve the associated data and make sure it remains available for eDiscovery cases. 

![Slide3](https://user-images.githubusercontent.com/104838111/235623468-c577287a-b9a0-4f38-8df8-9e86b5140799.png)
 
 
## 3 complementary options exist to apply rules    
1. Define and publish Retention Labels, so that Business Users can apply them to documents.  
2. Define Retention Labels, then specify a Policy to automatically apply these Labels to the appropriate content.  
3. Define a transparent Retention Policy (without a Label) and automatically apply this rule to the appropriate content.  

![Slide5](https://user-images.githubusercontent.com/104838111/235623738-f6854a4b-c59d-4e1b-8f6a-f8bf8b55f690.png)

## Labels - Summary
A File Plan consists in a set of Labels.  
Note: it is optional. You may directly define Labels.    
Every Label may include a disposition review step before data gets deleted.  
  
3 flavors of Labels exist:  
- "Standard" Retention Labels define a retention period and/or the need to delete the data after it expires
- Records prevent updates during the retention period
- Regulatory Records cannot be removed once they have been applied  

![Slide6](https://user-images.githubusercontent.com/104838111/235624088-1f93f661-a6de-491b-bbf3-e18420cb9545.png)

 
## Labels - More Details
The retention period can start after a specific Business Event.  
Users may unlock Records to temporarily authorize updates.  
Labels can embed various options (retain then trigger a disposition review, retain then re-label, retain forever...).  
A preservation lock can be applied to a Policy to freeze its definition and prevent admin updates.  
 
![Slide7](https://user-images.githubusercontent.com/104838111/235624375-8406e1e6-40ec-4a3f-ba78-99c8390105fc.png)

## Labels - PowerShell & APIs
Many PowerShell commands are available.   
For some specific admin tasks, they are even the only option available for the Administrator.  
Labels and Events can be managed with a dedicated Graph API.  

![image](https://user-images.githubusercontent.com/104838111/235638070-ac6de673-bd0c-4ca6-9d11-a04ba32a812d.png)

 
## Policies - Summary
DLM specifies a set of Retention Policies.
They may embark a Retention Label.
(1) Published Labels become visible for users in a set of M365 locations.  
(2) Labels can be automatically applied on documents in a set of locations. Additional filters can be applied, based on their content.  
(3) Transparent policies apply at the M365-container level (SPO site, ODB space, EXO mailbox...).  
 
DLM also includes a set of technical tools for Exchange Online (PST import, inactive mailboxes, archives).  

![Slide8](https://user-images.githubusercontent.com/104838111/235624575-883c416e-af47-4c41-961b-913e45c0e033.png)

## Policies - More Details
Policies apply to a scope (users, SPO locations or M365 group).  
These scopes may be static or dynamically re-evaluated. In this case, Microsoft calls them "adaptive scopes".  

![Slide9](https://user-images.githubusercontent.com/104838111/235624652-43e57a1b-7e51-4432-8e61-5d171f50d858.png)
