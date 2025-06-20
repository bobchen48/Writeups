# Road to Junos #
After coming off of my [CCNA](https://github.com/bobchen48/Writeups/blob/main/CCNA/My%20CCNA%20Journey.md) last month, I decided to hop into the Juniper landscape starting with JNCIA - Junos, which I was able to accomplish on April 28th. While CCNA to Juniper is not the biggest jump due to lots of overlaps in Networking fundamental knowledge, there still is a good deal of new terminologies (that are unique to Juniper) that I had to learn to adaquetely perpare for the exam

## Resources Used ##
1. **Udemy Course Juniper JNCIA-Junos JN0-105 by S2 Academy**: The main video course used for this certification exam. This video course broke the objectives mentioned on JNCIA - Junos Blueprint objectives into digestable video courses that can be consumed easily. I found this video course easy to follow.
  
2. **Juniper vLab**: A virtual lab environment that provides a virtualized environment to test commands in configuration mode. This was basically a close equivalent to Cisco Packet Tracer
   
3. **JNCIA-Junos JN0-105 Practice Exams by S2 Academy**: Complemtnary to S2 Academy's JNCIA Junos JN0-105. This provided me with 300 practice questions that I can practice to test my understand of Juniper CLI, OS, and Networking knowledge from a Juniper perspective. However, because of time constraint, I was only able to get through a third of the practice questions prior to taking my exam.
   
4. **Juniper JNCIA-Junos (JN0-105) - Practice Exam by Nerd Exam**: Similiar to JNCIA-Junos JN0-105 Practice Exams by S2 Academy by S2 academy, this practice exam course module provided an additional 100 practice questions to help me prepare for the Junos exam. But like the other practice exam course, I was not able to complete it all (only finished half) prior to exam date.

## Initial Preparation and Impressions (Comparing Cisco and Juniper) ##
When I first got into Juniper (and as I go through the lessons), I was not only taking notes of the stuff I was learning, but also taking mental notes of the differences I saw beteween Juniper and Cisco. Some notable differences I observed were as follows:
1. **Juniper SDN-lite architecture**: When I was first introduced to Juniper architecture in my video course, I immediately recalled the SDN architecture in Cisco. The way packets are forwarded between the control plane (Routing Engine) and Forwarding Plane (Forwarding Engine) was very similiar to how SDN Networking works at a foundational level (without the application plane). For me, this made it really easy to comprehend Juniper's architecture because the concepts of how packets flow in Juniper architecture was essentially the same as in an SDN architecture.
<div align="center">
  <image src="https://github.com/bobchen48/Writeups/blob/main/Juniper%20-%20Junos/SDN%20vs%20Juniper%20Architecture.JPG">
</div>

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
