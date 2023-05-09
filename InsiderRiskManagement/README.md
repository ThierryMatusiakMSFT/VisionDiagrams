# Insider Risk Management

Insider Risk Management monitors internal users activity to identify suspicious behaviors.


## Summary
Insider Risk Management (IRM) consists in a set of monitoring policies.  
They analyze activity and generate alerts.  
Reviewers can confirm relevant alerts into IRM Cases.  
Serious problems can result in formal investigations run in the eDiscovery module.  
IRM analyzes various sources of activity. 

![Slide3](https://user-images.githubusercontent.com/104838111/236775946-c9f9e5ef-d0f3-482e-a607-fb13e45161ec.png)


## Details
Data Connectors can feed IRM with additional information.  
Policies define who is monitored and what behaviors to monitor.  
Alerts can feed an external SIEM.  
Cases provide various tools : activity and content analysis, Teams collaboration, PowerAutomate actions,...  
  
![Slide4](https://user-images.githubusercontent.com/104838111/236776154-c8411c99-551b-477f-b3a0-c8ceb66f6c0b.png)


## Even more details...
You can configure various global IRM settings.  
IRM offers a dedicated audit Log to review IRM Admin activity.  
Forensics Evidence records Endpoint Activity.  
  
User Activity Reports allow to temporarily monitor users.  
IRM can feed DLP policies with Users’ Risk Level.  
  
Policy triggers initiate user's monitoring.  
Policy indicators accumulate and may result into raising an alert.  

![Slide5](https://user-images.githubusercontent.com/104838111/236776906-32326bc6-fd31-4b98-975a-ebd07c03ea53.png)


## Scoring Process
IRM policies analyse users’ activity over time.  
IRM may raise an alert, associated to a user. It also evaluates the severity of this alert (Low/Medium/High).  
An IRM policy consists in (at least) one triggering event and a set of indicators.  
The triggering event activates the IRM policy for a specific user.  
IRM starts collecting indicators and evaluates a severity for each of them.  
The IRM scoring engine also analyzes the audit log to score past activities.  
IRM raises an alert as soon as an indicator is suspicious.  
Further events aggregate into the same active alert.  
The scoring engine may also associate several indicators into a sequence.  
The scoring engine gives more importance to specified priority content.  
Cumulative activity identifies deviation from a “normal” pattern. It also influences the score.  
New indicators may change the severity of an existing alert.  
  
![Slide11](https://user-images.githubusercontent.com/104838111/172294252-272e53c1-5ccb-4dab-855d-652a0ad84241.JPG)






