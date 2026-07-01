# AWS Global Infrastructure
*Day 01 Notes* 

## Key Topics
- Regions
- Availability Zone
- Data Centers
- Edge Locations or Point of Presence (PoP)

### Regions

- Regions in aws are **global geographical areas contains multiple availbility zones (AZs).**
- **Three to Six AZs available in a region.**
- Choose regions based on **proximity, latency, data sovereignty laws to that specific country, avaliability of a service and pricing.**

***Example:** us-east-1, ap-south-1, ap-southeast-1, sa-east-1, etc.,*

### Availability Zone

- **Distinct, Isolated data centers** within a single aws region with **redundent power, networking, and connectivity.**
- **Atleast two or more data centers in a AZ.**
- Span atleast two availability zone for high availability.

### Point of Presence / Edge Location

- Globally distributed edge locations and regional caches used to bring cloud services, content and security closer to en-users location from actual location.

## TL;DR

- **Regions** are geographical area that has cluster of data centers in the name of AZs.
- **Availability Zone** are cluster of 2 or more discrete data centers. In a region, minimum 3 to 6 AZs available.
- **PoP/Edge Location** are cache and content distributed edge locations that shares data from regional data.

---
[Back to the README](/README.md) | *Content contributed by [Thanvir Assif](https://thanvirassif.com)* | [Next - (Day_02)]()