# Cybersecurity Incident Analysis

This repository contains an analysis of a DDoS attack on a multimedia company, following the NIST Cybersecurity Framework. It details the steps taken to identify, protect, detect, respond, and recover from the incident, serving as a valuable example for cybersecurity professionals and students.

### Incident Report Analysis - Example

You can find the detailed incident report [https://docs.google.com/document/d/1PHhXKN-gvCsVzfz8I0iODI-UEdASuvPTq6327LuZorI/edit?usp=sharing].

#### Summary
On the morning of May 25, our network services were disrupted for two hours due to a Distributed Denial of Service (DDoS) attack. The attack involved a flood of ICMP packets that overwhelmed our network, rendering internal network services inaccessible. The incident management team intervened by blocking incoming ICMP packets, shutting down non-critical services, and restoring critical ones. The cybersecurity team identified that the attack exploited an unconfigured firewall, allowing the malicious actor to flood our network with ICMP pings.

#### Identify
The cybersecurity team conducted an audit of our network infrastructure, systems, devices, and access policies to identify vulnerabilities. It was determined that the firewall lacked proper configuration, allowing the attacker to send a flood of ICMP packets. Additionally, the firewall did not verify source IP addresses, which could have mitigated the attack. To identify security risks, regular audits of internal networks, systems, devices, and access privileges were performed. These audits revealed that the firewall's configuration was insufficient to prevent the flood of ICMP packets. The lack of source IP verification allowed the attacker to use spoofed IP addresses, further exacerbating the issue.

#### Protect
The team has implemented new protective measures to prevent future attacks. These include adding rules to limit the rate of incoming ICMP packets and configuring the firewall to verify the authenticity of incoming IP addresses to prevent spoofed packets. Instituted mandatory training for all employees on recognizing and responding to potential cybersecurity threats. Developed and enforced new policies for network security and access control. Additionally, we deployed network monitoring software and an Intrusion Detection/Prevention System (IDS/IPS) to detect and filter malicious traffic.

#### Detect
To detect unauthorized access and abnormal traffic patterns in the future, the team has implemented continuous monitoring of network traffic for abnormal patterns, particularly focusing on detecting unusual spikes that could indicate a DDoS attack. We also installed IDS/IPS systems to identify and block malicious traffic, especially suspicious ICMP traffic. Enhanced logging and analysis of network activity, using Security Information and Event Management (SIEM) systems to correlate data and identify threats.

#### Respond
The team responded to the incident with the following actions: blocked incoming ICMP packets and isolated affected network segments. Notified upper management and relevant stakeholders about the incident. Ensured that all employees were informed and reminded of the procedures to follow during an attack. Conducted emergency training sessions for all staff on recognizing phishing attempts and other social engineering tactics to prevent credential compromise.

#### Recover
The team recovered affected systems by bringing critical network services back online after ensuring they were secure. Verified the integrity of our data and systems, ensuring no data loss occurred during the attack. Checked and verified the integrity of our backup systems to ensure they were not compromised. Recovering from the incident involved restoring affected systems to normal operation and verifying the integrity of our data. Regular backups were crucial in this process, allowing us to restore systems without data loss. This recovery phase ensured that our operations could resume swiftly and securely.

#### Reflections/Notes
The incident highlighted the need for a thorough review and continuous improvement of our firewall configurations and network security policies. Regular training and drills should be conducted to ensure all employees are prepared for potential security incidents. Future plans include investing in more advanced DDoS mitigation technologies and conducting regular vulnerability assessments to stay ahead of emerging threats. Collaboration with external cybersecurity experts could provide additional insights and recommendations to further strengthen our defenses. By addressing the gaps identified in this incident and implementing these measures, we aim to bolster our network security and reduce the risk of future attacks. Regular reviews, employee training, and advanced security measures will be critical in maintaining a robust security posture.
