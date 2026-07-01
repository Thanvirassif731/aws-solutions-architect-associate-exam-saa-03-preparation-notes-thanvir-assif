# AWS Global Infrastructure
*Day 01 Notes* 

## Key Topics
- Regions
- Availability Zone
- Data Centers
- Edge Locations or Point of Presence (PoP)
- Global vs. Regional Services
- Local Zones, Wavelength & Outposts

---

### Regions

- Regions in aws are **global geographical areas contains multiple availability zones (AZs).**
- **Three to Six AZs available in a region.**
- Choose regions based on **proximity, latency, data sovereignty laws to that specific country, avaliability of a service and pricing.**

***Example:** us-east-1, ap-south-1, ap-southeast-1, sa-east-1, etc.,*

### Availability Zone

- **Distinct, Isolated data centers** within a single aws region with **redundant power, networking, and connectivity.**
- **Atleast two or more data centers in a AZ.**
- Span atleast two availability zone for high availability.

### Point of Presence / Edge Location

- Globally distributed edge locations and regional caches used to bring cloud services, content and security closer to end-users location from actual location.

### Global vs. Regional Services

- Most AWS services are **Region-scoped**, meaning the data and resources are tied to a specific region and do not automatically replicate to others.
- **Global services** operate worldwide and their configurations apply across all regions simultaneously.

***Global Services Examples:** IAM, Route 53, CloudFront, WAF.*

***Regional Services Examples:** EC2, RDS, VPC, S3 (S3 is a global namespace but data is stored regionally).*

### AWS Local Zones

- Places AWS compute, storage, and database services closer to **large population, industry, and IT centers**.
- Acts as an extension of an AWS Region.
- Designed for applications requiring **single-digit millisecond latency** to end-users (e.g., real-time gaming, media & entertainment).

### AWS Wavelength

- Embeds AWS compute and storage services within **telecommunication providers 5G networks**.
- Eliminates the network hops required to reach AWS regions, providing **ultra-low latency** for mobile devices and end-users.

### AWS Outposts

- Fully managed service that brings native AWS infrastructure, services, APIs, and tools to virtually any **on-premises data center or co-location space**.
- Ideal for **hybrid cloud** architectures, local data processing, or legacy on-premises application integration.

## TL;DR

- **Regions** are geographical areas that have a cluster of data centers known as AZs.
- **Availability Zones** are clusters of 2 or more discrete data centers. In a region, a minimum of 3 to 6 AZs are available.
- **PoP/Edge Locations** are distributed cache locations that deliver content globally with low latency.
- **Service Scope:** Know your Global services (IAM, Route 53, CloudFront) vs. Regional services (EC2, VPC, Lambda).
- **Edge & Hybrid Compute:** **Local Zones** (closer to cities for single-digit latency),**Wavelength** (embedded in 5G networks), and **Outposts** (AWS infrastructure in your own on-premises data center).

---
[Back to the README](/README.md) | *Content contributed by [Thanvir Assif](https://thanvirassif.com)* | [Next - (Day_02)](/day_02.md)