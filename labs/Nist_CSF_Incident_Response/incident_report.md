# Cybersecurity Incident Report

## Summary

A large ICMP Flood attack overwhelmed the organization's internal network and caused network services to become unavailable for approximately two hours.

Investigation revealed that the attack was able to enter the network because of an improperly configured firewall.

The incident response team successfully restored critical services after blocking incoming ICMP traffic and disabling non-critical services.

## Attack Type 

ICMP Flood Attack

Course Exemplar Classification: ICMP flood Distributed Denial of Service (DDoS)

## Root Cause

An improperly configured firewall allowed excessive ICMP traffic into the internal network.

## Systems Affected

-  Internal network infrastructure
-  Critical network services
-  User access to internal resources

## Impact

-  Network service outage
-  Temporary business disruption
-  Loss of access to network resources

## Mitigation Actions

-  Blocked incoming ICMP traffic
-  Stopped non-critical services
-  Restored critical network services

## Security Enhancements

-  ICMP rate limiting
-  Firewall hardening
-  source IP verification
-  IDS/IPS implementation
-  Enhanced network monitoring

- ## 
