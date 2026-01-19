## Incident Summary

The organization experienced a Denial of Service (DoS) attack targeting its internal network infrastructure. The attack was carried out through a flood of ICMP packets, which overwhelmed network resources and caused critical services to become unresponsive.

The incident occurred earlier today and lasted for approximately two hours before being successfully contained. During the attack, the internal network was unable to process the excessive ICMP traffic, leading to a complete disruption of normal operations.

The affected organization is a multimedia company that provides web design, graphic design, and social media marketing services. Due to the nature of its business, the organization relies heavily on network availability, making the outage highly impactful to productivity and service delivery.

Investigation revealed that the attack was enabled by a misconfigured firewall that lacked proper controls to limit ICMP traffic. As a result, the malicious traffic was allowed to flood the network without restriction.

To mitigate the incident, the incident response team blocked incoming ICMP packets, disabled non-critical network services, and restored critical services. These actions successfully stabilized the network and allowed essential operations to resume.
