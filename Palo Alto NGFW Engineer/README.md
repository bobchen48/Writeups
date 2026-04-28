# Palo Alto Next-Generation Firewall Engineer - Pushing through failure #
On 4-28-2026, I was able to clear the [Palo Alto Next Generation Firewall Engineer Certification](https://www.paloaltonetworks.com/services/education/palo-alto-networks-ngfw-engineer). This was one of the most frustrating exam I have taken in a good while since [Broadcom VCP-VCF (Vmware Cloud Foundation) that I failed back in July 2025](https://github.com/bobchen48/Writeups/tree/main/VCP%20-%20VCF%20(VMware%20Cloud%20Foundation)%205.2). It taught me that if you really want something in the event of a setback, you must have that will to push through it

## Resources Used ##
1. **[Palo Alto Learn (Beacon)](https://learn.paloaltonetworks.com/learn)**: Main resource I used for this certification. This was Palo Alto's official learning platform for all of their certifications, products, features, etc. Given there was a limited publically available resources I had to prepare for this certification, this was the most important resource one that exposed me to many high level concept for this exam.
  
2. **Hands-on configuration**: Since I work with Palo Alto professionally, I had hands-on experience configuring Security Policies, NAT, basic administration on Panorama since 2025.
   
3. **[Palo Alto NGFW Engineer Datasheet](https://www.paloaltonetworks.com/content/dam/pan/en_US/assets/pdf/datasheets/education/ngfw-engineer-datasheet.pdf)**: I wish I referred to this exam datasheet the first time I took it because it ended up being more helpful than I gave it credit for. I will elaborate how I used this later on this blog
   
4. CBTNuggets PCNSA & PCNSE by Keith Barker: Since I did not do PCNSA or PCNSE (having only completed a PCCET) before all of them retired, I figured this would still be a good video series to knock out as part of my initial preparation. While I was able to knock out most of PCNSA, I only got through PCNSE partially before putting this course down in favor of the official Palo Alto Learning Platform. Regardless, these two courses were still helpful giving me exposure into high-level content idea for some of the NGFW Engineer topics as there was a fair amount of overlap in exam topic between PCNSA/PCNSE and new NGFW Engineer exam
   
5. **Udemy Course: Palo Alto Networks Next-Generation Firewall Engineer - Exams by Paweł Krakowiak**: I was initially skeptical of this resource because of the mixed reviews by many test takers had given that it did not adaquetly prepare you for the real exam. However, after failing it the first time, I purchased this practice exam course and to my surprise, it revealed big gap in 2 domains I had: SSL/TLS Profile (Certificate Profile, SSL Forward Proxy) & GlobalProtect
   
6. **[Wesley Cyber NGFW Engineer Playlist](https://www.youtube.com/playlist?list=PLltJsgfsuLOit54c49FkjTx2-51S5nVdI)**: Although this playlist is incomplete, I watched the first 3 videos prior to my first attempt and THOROUGHLY gone through the full playlist prior to my 2nd re-attempt. Given that Wes covered most of Domain 1: PAN-OS Networking Configuration, I rate his YouTube series highly valueable being able to watch him configure things hands on
7. INE Palo Alto Labs: This was more of an impulsive buy. I can't attest 100 percent that I needed it, but every little bit helps

## Background and initial preparation ##
Back in Jan 2025, I took (now-retired) Palo Alto Certified Cybersecurity Entry Level Technician (PCCET) as my entry point into the world of Palo Alto NGFW. While PCCET was not technical, I still appreciated the learning experience. However, because [PCCET, PCNSA, and shortly-after PCNSE were retired](https://live.paloaltonetworks.com/t5/news/new-security-service-edge-engineer-certification-upcoming/ta-p/997555) by 2026 in favor of role-based exams, I was unable to test myself against PCNSA content. After reviewing several of the new role-based certification as well as what online community feedback, I decided that NGFW Engineer exam was the most appropriate exam to pursue given its scope. I began studying in November 2025.

I started with CBT Nuggets PCNSA and PCNSE course by Keith Barker to build foundational knowledge. Since it was winter, I gave myself until Spring 2026 to prepare rather than rushing to complete it within one to two months, as I wanted a slower steady appraoch and did not want to go out during the winter season. While I initially progressed at at a decent pace and was able to complete the PCNSA course, I found PCNSE content - nearly double PCNSA, to be overwhelming. Halfway through PCNSE, I decided to drop it in favor of learning from the official Palo Alto Learn platform when January 2026 came around and I realized I needed to pick up the pace.

I then switched to Palo Alto Learning platform (formerly Beacon), focusing on reviewing high-level concepts such as interface types, HA setup, routing, and switching. This is where things got interesting, as I was being introduced to cloud NGFW concepts (VM-Series, CN-Series, Cloud Identity Engine, AI Runtime Security, and more), much of which were unfamiliar.

Fortunately, because I had completed AZ-900 and the AWS Cloud Practitioner certification, I was okay comprending with many high-level cloud concepts that Palo Alto integrates with (such as Azure VNet and AWS VPC). My main gap was Google Cloud integration.

Throughout the process, I built my a Quizlet flashcard deck to review key concepts. I found this especially valueable for reviewing via spaced repetition.

## First Attempt ##
After I finished the Palo Alto learning course and first two videos of WesleyCyber's NGFW playlist that he released, I went in for my first attempt into the exam.

As I went through the exam, a steady sense of unease set in. Many questions left me uncertain—I could narrow them down to two choices, but it often came down to a 50–50 guess. In the end, I failed.

## Reviewing Exam Result and Determining next step ## 
While I wasn’t surprised, given my limited resources, I was still frustrated by the outcome and the percentages in my results. Frustrated, I went home and pulled up the Exam Datasheet, copying it into a Google Doc. I then commented on every topic listed under each subdomain that I was uncomfortable with.

Shortly after, I impulsively bought an INE course because it was on sale and included Palo Alto labs for extra practice. It wasn’t the wisest decision, but I justified it by planning to pursue JNCIP-ENT later in the year and making use of it one way or another.

Throughout my review, I watched WesleyCyber’s NGFW YouTube series. Although the videos only covered Domain 1 at the time, I found them helpful, especially since I scored 50% in that domain.

Additionally, I built out my Google Doc notes by adding hyperlinks and referencing relevant Palo Alto TechDocs for each topic I found useful. Soon after, I had a fully built-out  exam datasheet–based notes, highlighting key concepts I needed to review prior to retake. I skipped Domain 3: Integration and Automation, as I performed best in it on my first attempt (80%) and it had the lowest weighting (20%).

## Second Attempt ##
After reviewing everything for a month, I went in for my 2nd attempt, feeling much more confident about what I got wrong the first time. I confidently went through the questions, reading word for word to make sure I understand what I was being asked of. Thanks to the Exam Datasheet notes I took, I was able to pass it the 2nd go-round

## Advice to Others ##

**Understand CCNA-level knowledge, Security+, and Basic Cloud Concepts** : While the exam does not have any real pre-requisite, it implies and demands a working (CCNA-level Networking knowledge), basic Security+ knowledge, and basic Cloud (Azure and AWS mostly) knowledge. Knowing how these work together in tandem with Palo Alto (especially concerning deploying VM-series Firewall) will increase your chances of success.
   



