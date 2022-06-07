# Insider Risk Management

Insider Risk Management monitors internal users activity to identify suspicious behaviors.


## Summary
Insider Risk Management (IRM) consists in a set of monitoring policies.<BR/>
They analyze activity and generate alerts.<BR/>
Reviewers can confirm relevant alerts into IRM Cases.<BR/>
Serious problems can result in formal investigations run in the eDiscovery module.<BR/>
<BR/>
![Slide3](https://user-images.githubusercontent.com/104838111/172293958-7a1ccab7-7340-4605-9d64-5f9c88eeb030.JPG)


## Details
Data Connectors can feed IRM with additional information.<BR/>
Policies define who is monitored and what behaviors to monitor.<BR/>
Alerts can feed an external SIEM.<BR/>
Cases provide various tools : activity and content analysis, Teams collaboration, PowerAutomate actions,...<BR/>
<BR/>
![Slide4](https://user-images.githubusercontent.com/104838111/172294012-e76bcf2c-f692-45b0-9abf-6f5750b93001.JPG)


## Even more details...
You can configure various global IRM settings.<BR/>
IRM offers a dedicated audit Log.<BR/>
Policy triggers initiate user's monitoring.<BR/>
Policy indicators accumulate and may result into raising an alert.<BR/>
<BR/>
![Slide5](https://user-images.githubusercontent.com/104838111/172294040-62f8d199-d831-41b1-a157-7f48b6c07a4d.JPG)


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
![Slide11](https://user-images.githubusercontent.com/104838111/172294252-272e53c1-5ccb-4dab-855d-652a0ad84241.JPG)






