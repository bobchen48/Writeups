# Palo Alto Next-Generation Firewall Engineer - Pushing through failure #
On 4-28-2026, I was able to clear the [Palo Alto Next Generation Firewall Engineer Certification](https://www.paloaltonetworks.com/services/education/palo-alto-networks-ngfw-engineer). 

## Resources Used ##
1. **[Palo Alto Learn (Beacon)](https://learn.paloaltonetworks.com/learn)**: Main resource I used for this certification. This was Palo Alto's official learning platform for all of their certifications, products, features, etc. Given there was a limited publically available resources I had to prepare for this certification, this was the most important resource one that exposed me to many high level concept for this exam.
  
2. **Hands-on configuration**: Since I work with Palo Alto professionally, I had hands-on experience configuring Security Policies, NAT, basic administration on Panorama since 2025.
   
3. **[Palo Alto NGFW Engineer Datasheet](https://www.paloaltonetworks.com/content/dam/pan/en_US/assets/pdf/datasheets/education/ngfw-engineer-datasheet.pdf)**: I wish I referred to this exam datasheet the first time I took it because it ended up being more helpful than I gave it credit for. I will elaborate how I used this later on this blog
   
4. CBTNuggets PCNSA & PCNSE by Keith Barker: Since I did not do PCNSA or PCNSE (having only completed a PCCET) before they retired, I figured this would still be a good video series to knock out as part of my initial preparation. While I was able to knock out most of PCNSA, I only got through PCNSE partially before putting this course down in favor of the official Palo Alto Learning Platform. Regardless, these two courses were still helpful giving me exposure into high-level content idea for some of the NGFW Engineer topics as there was a fair amount of overlap in exam topic between PCNSA/PCNSE and new NGFW Engineer exam
   
5. **Udemy Course: Palo Alto Networks Next-Generation Firewall Engineer - Exams by Paweł Krakowiak**: I was initially skeptical of this resource because of the mixed reviews by many test takers had given that it did not adaquetly prepare you for the real exam. However, after failing it the first time, I purchased this practice exam course and to my surprise, it revealed big gap in 2 domains I had: SSL/TLS Profile (Certificate Profile, SSL Forward Proxy) & GlobalProtect
   
6. **[Wesley Cyber NGFW Engineer Playlist](https://www.youtube.com/playlist?list=PLltJsgfsuLOit54c49FkjTx2-51S5nVdI)**: Although this playlist is incomplete, I watched the first 3 videos prior to my first attempt and THOROUGHLY gone through the full playlist prior to my 2nd re-attempt. Given that Wes covered most of Domain 1: PAN-OS Networking Configuration, I rate his YouTube series highly valueable being able to watch him configure things hands on

## Background and initial preparation ##
When I first got into Juniper (and as I go through the lessons), I was not only taking notes of the stuff I was learning, but also taking mental notes of the differences I saw beteween Juniper and Cisco. Some notable differences I observed were as follows:
1. **Juniper SDN-lite architecture**: When I was first introduced to Juniper architecture in my video course, I immediately recalled the SDN architecture in Cisco. The way packets are forwarded between the control plane (Routing Engine) and Forwarding Plane (Forwarding Engine) was very similiar to how SDN Networking works at a foundational level (without the application plane). For me, this made it really easy to comprehend Juniper's architecture because the concepts of how packets flow in Juniper architecture was essentially the same as in an SDN architecture.


2. **Cisco vs Juniper CLI**: I found Juniper CLI to be more object-oriented and "flat" than Cisco's more layered approach. While in the vLab executing commands (as I go through lessons), I felt that Juniper was very straight forward configuration wise in that once I was in the configuration mode, I can either execute a full command to accomplish a task from edit, or I can go into edit-(insert specific object group), thus making it more straight forward and logically sectioned out.
   
3. **Terminology Differences** While Network fundamentals don't change across vendors, Juniper and Cisco's history and design methodology causes them to adopt different terminologies that mean the same thing. For example:
   - VRF (Cisco) == Routing Instance (Juniper)
   - Running Config & Startup Config (Cisco) == Active Configuration & Candidate Configuration (Juniper)
   - Administrative Distance (Cisco) == Route Preference (Juniper)

  These were some important distinction I had to keep in mind when studying because my mind would naturally be oriented towards Cisco terminologies, which then led to me having to remind myself to apply a Juniper mindset, especially as I got closer to the exam date 
  
4. **Cisco Administrative Distance (aka Juniper Route Preference) Differences**
After studying for CCNA for so long and having my brain hard-wired into associating OSPF with 110, RIP with 120, IS-IS with 125 for their default administrative distance, I was having difficulties adopting into Juniper's differences in their Route preference value as I saw OSPF with 150, RIP with 100, IS-IS (which has 2 levels described by Juniper) with 160 for level 1 external and 165 for level 2 external. While you may not necessarily need to memorize each routing protocol's default route preference for JNCIA - Junos (don't quote me on that), I am almost certain that as I move into JNCIS - SP and JNCIS - Enterprise I will need to memorize them.


## Crunching for Time and Exam Date
While I was comfortably cracking through the training videos, I found it difficult to manage my time as I got closer to the exam among other priorities (I was also preparing for finals around this time) that I found myself rushing through some of the videos closer towards my exam date. Up to 2 days before the exam, I was simply rushing through the final set of videos and banking on my Cisco CCNA knowledge to carry me through a big portion of the exam. 

## Advice to Others ##
1. **Get comfortable with Juniper CLI** : Regardless of whether you have CCNA or not, you should be able to comfortably navigate through CLI of a Junos device prior to taking this exam as this exam is mostly split towards 60 percent understanding Junos CLI and 40 percent networking fundamentals.
   
2. **Subnetting**: Like my CCNA test-taking recommendation, Subnetting knowledge is a must. Knowing subnetting helps you understand how routes are chosen when there are multiple routes to choose from to a destination IP (most specific aka Longest matching route) win


