# Palo Alto Next-Generation Firewall Engineer - Pushing through failure #
On 4-28-2026, I was able to clear the [Palo Alto Next Generation Firewall Engineer Certification](https://www.paloaltonetworks.com/services/education/palo-alto-networks-ngfw-engineer). This was one of the most frustrating exam I have taken in a good while since [Broadcom VCP-VCF (Vmware Cloud Foundation) that I failed back in July 2025](https://github.com/bobchen48/Writeups/tree/main/VCP%20-%20VCF%20(VMware%20Cloud%20Foundation)%205.2). It taught me the importance of viewing failure as a temporary setback, not an identity in the event where if you really want to achieve something that holds a feeling of mastery, you will push through failure

## Resources Used ##
1. **[Palo Alto Learn (Beacon)](https://learn.paloaltonetworks.com/learn)**: Main resource I used for this certification. This was Palo Alto's official learning platform for all of their certifications, products, features, etc. Given there was a limited publically available resources I had to prepare for this certification, this was the most important resource one that exposed me to many high level concept for this exam.
  
2. **Hands-on configuration**: Since I work with Palo Alto professionally, I had hands-on experience configuring Security Policies, NAT, basic administration on Panorama since 2025.
   
3. **[Palo Alto NGFW Engineer Datasheet](https://www.paloaltonetworks.com/content/dam/pan/en_US/assets/pdf/datasheets/education/ngfw-engineer-datasheet.pdf)**: I wish I referred to this exam datasheet the first time I took it because it ended up being more helpful than I gave it credit for. I will elaborate how I used this later on this blog
   
4. CBTNuggets PCNSA & PCNSE by Keith Barker: Since I did not do PCNSA or PCNSE (having only completed a PCCET) before they retired, I figured this would still be a good video series to knock out as part of my initial preparation. While I was able to knock out most of PCNSA, I only got through PCNSE partially before putting this course down in favor of the official Palo Alto Learning Platform. Regardless, these two courses were still helpful giving me exposure into high-level content idea for some of the NGFW Engineer topics as there was a fair amount of overlap in exam topic between PCNSA/PCNSE and new NGFW Engineer exam
   
5. **Udemy Course: Palo Alto Networks Next-Generation Firewall Engineer - Exams by Paweł Krakowiak**: I was initially skeptical of this resource because of the mixed reviews by many test takers had given that it did not adaquetly prepare you for the real exam. However, after failing it the first time, I purchased this practice exam course and to my surprise, it revealed big gap in 2 domains I had: SSL/TLS Profile (Certificate Profile, SSL Forward Proxy) & GlobalProtect
   
6. **[Wesley Cyber NGFW Engineer Playlist](https://www.youtube.com/playlist?list=PLltJsgfsuLOit54c49FkjTx2-51S5nVdI)**: Although this playlist is incomplete, I watched the first 3 videos prior to my first attempt and THOROUGHLY gone through the full playlist prior to my 2nd re-attempt. Given that Wes covered most of Domain 1: PAN-OS Networking Configuration, I rate his YouTube series highly valueable being able to watch him configure things hands on

## Background and initial preparation ##
Back in Jan 2025, I took (now-retired) Palo Alto Certified Cybersecurity Entry Level Technician (PCCET) as my entry point into the world of Palo Alto NGFW. While PCCET was no-where technical, I still appreciated the experience learning it. However, because [PCCET, PCNSA, and shortly-after PCNSE were retired](https://live.paloaltonetworks.com/t5/news/new-security-service-edge-engineer-certification-upcoming/ta-p/997555) in favor of role-based exams, I was not able to test myself against PCNSA content. After reviewing several of the new role-based certification as well as what online forums had to say about them, I determined that NGFW Engineer exam was the most appropriate exam to pursue given its scope. So I started preparation in November 2025

I started by watching CBTNuggets PCNSA and PCNSE course by Keith Barker to absorb in as much of the conceptual knowledge as I could. Because it was the winter season, I gave myself until Spring 2026 to prepare instead of relying on an aggressive approach to get it within 1 to 2 months because I did not want to go out during the winter season to take any exam and I want to take this one a bit more slowly. While I felt like I was initially going at a decent pace and was able to complete the PCNSA course, the sheer volume of content in PCNSE (almost double of PCNSA) I found to be too much so halfwaythrough PCNSE, I decided to drop it in favour of the learning from the official learning platform once January 2026 came around and I realized I needed to step up the pace.

I then opened the Palo Alto Learning (formerly known as Beacon) and continued forward, reviewing important high-level concept such as Interface Types, HA setup, Routing and Switching. This was where things got interesting as I started also gaining exposure to cloud NGFW concepts (VM-series, CN-series, Cloud Identity Engine, AI Runtime security, and many more), which completely blew me away because I was very unfamamiliar with a lot of it. Thankfully, because I had previously completed AZ-900 and AWS Cloud Practitioner, I was comfortable enough with many of the high-level cloud-specific concepts that Palo integrates with (such as Azure VNet, AWS VPC); only one I had no real understanding of was the Google Cloud. One thing I also want to note was that as I was going through the Palo Alto Learning platform, I was building my own Quizlet flashcard deck of concepts to review throughout the lifecycle of the exam. I thought this was important because it gave me a flashcard repository that I can periodically go through and casually review daily to ensure I remember the concepts that I learned via spaced repetition

## First Attempt ##
After I finished the Palo Alto learning course and first two video of WesleyCyber's NGFW playlist that he released, I (having committed to March 2026) went in for my first attempt into the exam, still not ensure what to expect of it. 

As I went through the exam, I can feel the unsettling motion going through my body

##  ##
While I was comfortably cracking through the training videos, I found it difficult to manage my time as I got closer to the exam among other priorities (I was also preparing for finals around this time) that I found myself rushing through some of the videos closer towards my exam date. Up to 2 days before the exam, I was simply rushing through the final set of videos and banking on my Cisco CCNA knowledge to carry me through a big portion of the exam. 

## Advice to Others ##
1. **Get comfortable with Juniper CLI** : Regardless of whether you have CCNA or not, you should be able to comfortably navigate through CLI of a Junos device prior to taking this exam as this exam is mostly split towards 60 percent understanding Junos CLI and 40 percent networking fundamentals.
   
2. **Subnetting**: Like my CCNA test-taking recommendation, Subnetting knowledge is a must. Knowing subnetting helps you understand how routes are chosen when there are multiple routes to choose from to a destination IP (most specific aka Longest matching route) win


