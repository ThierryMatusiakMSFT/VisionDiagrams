# Data Lifecycle Management & Records Management

Data Lifecycle Management (DLM) protects important data during its retention period. 
It can also erase old data. 

Records Management extends DLM to prevent records updates or deletion.

## Context
Compliance Officers define a set of Retention Labels and Retention Policies.  
These policies include a data retention period (in case a user deletes this content).  
They can also result into documents' deletion after a specific period. This deletion can be automatic or go through a disposition review.  
Both Records Management and Data Lifecycle Management apply to M365 Data.  
M365 uses dedicated storage locations to preserve the associated data and make sure it remains available for eDiscovery cases.  
  
![Slide3](https://user-images.githubusercontent.com/104838111/183934326-4e3e6492-34a4-46a1-a72c-57a6b2276dd4.png)

## 3 complementary options exist to apply rules    
1. Define and publish Retention Labels, so that Business Users can apply them to documents.  
2. Define Retention Labels, then specify a Policy to automatically apply these Labels to the appropriate content.  
3. Define a transparent Retention Policy (without a Label) and automatically apply this rule to the appropriate content.  
  
![Slide4](https://user-images.githubusercontent.com/104838111/183939212-98c54687-243d-4c0b-a63f-1cdcc3a08e95.png)

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
  
![Slide6](https://user-images.githubusercontent.com/104838111/183941970-f7041197-31aa-49ff-9594-28bf1680f467.png)

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
