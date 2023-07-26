> This report is produced for demonstration purposes only and illustrates how to create a CTI Report using CTI Templates from Center for Threat Informed Defense. Orgininal template: https://github.com/center-for-threat-informed-defense/cti-blueprints/blob/main/samples/CTID%20Executive%20Sample%20Report.pdf

# Executive Report

## Business-Critical Processes Targeted by Multiple Threat Actors

### Febuary 1, 2023

@[tag](tlp:green) @[tag](misp-galaxy:threat-actor="TA577")

---

## Executive Summary

OneNote is increasingly being leveraged to distribute malware by cyber criminals. The reliance on 
sharing data via OneNote in the company to encourage collaboration makes our users susceptible 
to this new initial intrusion vector and threat actors are leveraging legitimate Microsoft services to 
send OneNote files that contain malware. Unlike traditional forms of phishing, training is unlikely to 
be an effective mitigation as business process involves the expectation of OneNote links to be sent 
via email.

## Key Points

* Over the last four months there has been a large increase in the use of Microsoft OneNote documents to successfully deliver malware. 
* This increase is likely attributed to Microsoft blocking macros by default in Microsoft Office applications in 2022 due to long-term abuse by threat actors.
* Employee awareness training is unlikely to substantially reduce our vulnerability to this new 
method of exploitation because users are conditioned to click OneNote links sent to them via 
Microsoft addresses.

---

## ASSESSMENT

We now face increased risk because cyber threat actors are targeting Microsoft OneNote, which is 
critical to our regular business operations. OneNote abuse poses a larger risk than malicious Word 
or Excel documents did prior to the macro change because we did not rely on macros for business 
processes. The new technique is effective in bypassing detection, introducing gaps in our threat 
detection coverage.

* Reports show multiple OneNote malware samples are going undetected by many anti-virus vendors including our current security stack. In January 2023, Proofpoint observed over 50 OneNote campaigns delivering different undetected malware payloads. Both lures and first stage implants have effectively evaded 
detection.

External researchers “assess with high confidence this is one of the largest email threat landscape shifts in 
recent history.”

* TA577’s adoption of OneNote is an early indicator that other more sophisticated actors will begin using this 
technique soon. TA577 is an initial access broker that facilitates follow-on infections for additional malware 
including ransomware.

---

## OUTLOOK

Increased use of this vector is likely to continue, threatening our defenses and business-critical 
processes. Technical mitigations are currently limited as our security tools do not currently detect 
malicious OneNote files and maintaining a whitelist for collaboration is likely to cause too many 
business interruptions. Long-term consideration should be given to adapting business processes to 
reduce risk exposure. 

--- 

## KEY INTELLIGENCE GAPS

* What is the scope and scale of OneNote delivery of malware?
* What is the breakdown of effects related to this initial intrusion vector? What is our risk exposure 
to those?

---

## INTELLIGENCE REQUIREMENTS

* What vulnerabilities are currently being exploited in the wild? 
* What exploited vulnerabilities can our organization detect?
* Identify and research threat actors targeting similar organizations. 
* Identify and research tools and malware used by threat actors targeting similar organizations.

---

## DATA SOURCES

* @[attribute](b970b288-d739-46b4-9d14-4a0934ee5f58)
* @[attribute](4f8c9bd8-b707-426c-b9a6-8353c04d4e6b)
* @[attribute](3f0550ce-6023-432f-b4c9-e7d708c93044)

---

## PROBABILITY MATRIX

| ALMOST NO CHANCE | VERY UNLIKELY | UNLIKELY | ROUGHLY EVEN CHANCE | LIKELY | VERY LIKELY | ALMOST CERTAINLY |
| -------- | -------- | -------- | -------- | -------- | -------- | -------- |
| remote     | highly improbable     | improbable     | roughly even odds     | probable     | highly probable     | nearly certain |
| 01-05% | 05-20% | 20-45% | 45-55% | 55-80% | 80-95% | 95-99 |
