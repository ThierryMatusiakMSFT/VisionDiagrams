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
- Define and publish Retention Labels, so that Business Users can apply them to documents.  
- Define Retention Labels, then specify a Policy to automatically apply these Labels to the appropriate content.  
- Define a transparent Retention Policy (without a Label) and automatically apply this rule to the appropriate content.  

![Slide5](https://user-images.githubusercontent.com/104838111/235623738-f6854a4b-c59d-4e1b-8f6a-f8bf8b55f690.png)

## Labels - Summary
A File Plan consists in a set of Labels.  
Note: it is optional. You may directly define Labels.    
Every Label may include a disposition review step before data gets deleted.  
  
3 flavors of Labels exist:  
- "Standard" Retention Labels define a retention period and/or the need to delete the data after it expires
- Records prevent updates during the retention period. Users may unlock Records to temporarily authorize updates.  
- Regulatory Records cannot be removed once they have been applied  

Every Label definition specifies various options : the retention period, when to start counting, what to do when data expires...

![Slide6](https://user-images.githubusercontent.com/104838111/235660231-b2523454-ebbb-453b-86f4-afad044d7f67.png)

 
## Labels - More Details
The retention period may start after a specific Business Event.    
Admins can explore labels usage in the console.  

They define Retention policies associated to these Labels.  
A preservation lock can be applied to a Policy to freeze its definition and prevent admin updates.  

3 flavors of Retention Policies exist, 2 of them being associated to a Label.

![Slide7](https://user-images.githubusercontent.com/104838111/235624375-8406e1e6-40ec-4a3f-ba78-99c8390105fc.png)

## Labels - PowerShell & APIs
Many PowerShell commands are available.   
For some specific admin tasks, they are even the only option available for the Administrator.  
Labels and Events can also be managed with a dedicated Graph API.  

![Slide8](https://user-images.githubusercontent.com/104838111/235638070-ac6de673-bd0c-4ca6-9d11-a04ba32a812d.png)

 
## Policies - Summary
DLM specifies a set of Retention Policies.  
They may embark a Retention Label.  
  
- Published Labels become visible for users in a set of M365 locations.  
- Labels can also be automatically applied on documents in a set of locations. Additional filters can be applied, based on their content.  
- Transparent policies apply at the M365-container level (SPO site, ODB space, EXO mailbox...).  
 
DLM also includes a set of technical tools for Exchange Online (PST import, inactive mailboxes, archives).  

![Slide9](https://user-images.githubusercontent.com/104838111/235660347-0360bb1a-45a3-4a81-b9fa-fe44949f613c.png)

## Policies - More Details
Policies apply to a scope. It may be static or dynamic (users, SPO locations or M365 group).  
These scopes may be static or dynamically re-evaluated (aka "adaptive scopes").  

Every policy type includes its own set of options.  

EXO tools include MRM policies and litigation holds.  

![Slide10](https://user-images.githubusercontent.com/104838111/235660680-9a7949f9-82d8-47c5-a97d-313b005a1180.png)

