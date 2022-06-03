# Insider Risk Management

Insider Risk Management monitors internal users activity to identify suspicious behaviors.


## Summary
Insider Risk Management (IRM) consists in a set of monitoring policies.<BR/>
They analyze activity and generate alerts.<BR/>
Reviewers can confirm relevant alerts into IRM Cases.<BR/>
Serious problems can result in formal investigations run in the eDiscovery module.<BR/>
<BR/>
![image](https://user-images.githubusercontent.com/104838111/171820381-cdc47efa-e6b5-41eb-bb79-c299b86de9b1.png)

## Details
Data Connectors can feed IRM with additional information.<BR/>
Policies define who is monitored and what behaviors to monitor.<BR/>
Alerts can feed an external SIEM.<BR/>
Cases provide various tools : activity and content analysis, Teams collaboration, PowerAutomate actions,...<BR/>
<BR/>
![image](https://user-images.githubusercontent.com/104838111/171820407-bfc93bb4-dd37-4c6f-85b0-938fb6e32e29.png)


## Even more details...
You can configure various global IRM settings.<BR/>
IRM offers a dedicated audit Log.<BR/>
Policy triggers initiate user's monitoring.<BR/>
Policy indicators accumulate and may result into raising an alert.<BR/>
<BR/>
![image](https://user-images.githubusercontent.com/104838111/171820443-54572312-da1a-4b87-bb2e-bf09971e1b7c.png)


## Scoring Process
IRM policies analyse users’ activity over time.<BR/>
IRM may raise an alert, associated to a user. It also evaluates the severity of this alert (Low/Medium/High).<BR/>
An IRM policy consists in (at least) one triggering event and a set of indicators.<BR/>
The triggering event activates the IRM policy for a specific user.<BR/>
IRM starts collecting indicators and evaluates a severity for each of them.<BR/>
The IRM scoring engine also analyzes the audit log to score past activities.<BR/>
IRM raises an alert as soon as an indicator is suspicious.<BR/>
Further events aggregate into the same active alert.<BR/>
The scoring engine may also associate several indicators into a sequence.<BR/>
The scoring engine gives more importance to specified priority content.<BR/>
Cumulative activity identifies deviation from a “normal” pattern. It also influences the score.<BR/>
New indicators may change the severity of an existing alert.<BR/>
<BR/>
![image](https://user-images.githubusercontent.com/104838111/171823679-6408ab88-21fd-498c-9ce2-6d53aea83116.png)






