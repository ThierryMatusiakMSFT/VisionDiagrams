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
![Slide3](https://user-images.githubusercontent.com/104838111/235620695-628a1819-0c98-4180-b083-f8a284277b20.png)
  
## 3 complementary options exist to apply rules    
1. Define and publish Retention Labels, so that Business Users can apply them to documents.  
2. Define Retention Labels, then specify a Policy to automatically apply these Labels to the appropriate content.  
3. Define a transparent Retention Policy (without a Label) and automatically apply this rule to the appropriate content.  
![Slide5](https://user-images.githubusercontent.com/104838111/235620873-593e25d2-e907-4edd-8d89-3cc633198122.png)
  
## Labels - Summary
A File Plan consists in a set of Labels.  
Note: it is optional. You may directly define Labels.    
Every Label may include a disposition reivew step before data gets deleted.  
  
3 flavors of Labels exist:  
- "Standard" Retention Labels define a retention period and/or the need to delete the data after it expires
- Records prevent updates during the retention period
- Regulatory Records cannot be removed once they have been applied  
  
![Slide5](https://user-images.githubusercontent.com/104838111/183939377-652d41af-9d07-4ddf-8012-f06d29e47249.png)

## Labels - More Details
The retention period can start after a specific Business Event.  
Users may unlock Records to temporarily authorize updates.  
Labels can embed various options (retain then trigger a disposition review, retain then re-label, retain forever...).  
Labels and Events can be managed with a dedicated Graph API.  
  
![Slide6](https://user-images.githubusercontent.com/104838111/184108068-bfa08303-ec6c-457a-982e-b5f1123dbfc5.png)

## Policies - Summary
Policies apply to a scope (users, SPO locations or M365 group).  
These scopes may be static or dynamically re-evaluated. Microsoft calls them "adaptive".  
DLM also includes a set of technical tools for Exchange Online (PST import, inactive mailboxes, archives).  


![Slide7](https://user-images.githubusercontent.com/104838111/183945579-5f8a5bcd-da48-40c5-9d9a-6634dd37f646.png)

## Policies - More Details
A preservation lock can be applied to a Policy to freeze its definition and prevent admin updates.  
(1) Published Labels become visible for users in a set of M365 locations.  
(2) Labels can be automatically applied on documents in a set of locations. Additional filters can be applied, based on their content.  
(3) Transparent policies apply at the M365-container level (SPO site, ODB space, EXO mailbox...).  
  
![Slide8](https://user-images.githubusercontent.com/104838111/183946362-ace139c1-183d-4a5a-a7b0-8e6bdc72e892.png)
