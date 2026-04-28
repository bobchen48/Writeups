# Palo Alto Next-Generation Firewall Engineer - Pushing through failure #
On 4-28-2026, I was able to clear the [Palo Alto Next Generation Firewall Engineer Certification](https://www.paloaltonetworks.com/services/education/palo-alto-networks-ngfw-engineer). This was one of the most frustrating exam I have taken in a good while since [Broadcom VCP-VCF (Vmware Cloud Foundation) that I failed back in July 2025](https://github.com/bobchen48/Writeups/tree/main/VCP%20-%20VCF%20(VMware%20Cloud%20Foundation)%205.2). It taught me the importance of viewing failure as a temporary setback, not an identity in the event where if you really want to achieve something that holds a feeling of mastery, you will push through failure

## Resources Used ##
1. **[Palo Alto Learn (Beacon)](https://learn.paloaltonetworks.com/learn)**: Main resource I used for this certification. This was Palo Alto's official learning platform for all of their certifications, products, features, etc. Given there was a limited publically available resources I had to prepare for this certification, this was the most important resource one that exposed me to many high level concept for this exam.
  
2. **Hands-on configuration**: Since I work with Palo Alto professionally, I had hands-on experience configuring Security Policies, NAT, basic administration on Panorama since 2025.
   
3. **[Palo Alto NGFW Engineer Datasheet](https://www.paloaltonetworks.com/content/dam/pan/en_US/assets/pdf/datasheets/education/ngfw-engineer-datasheet.pdf)**: I wish I referred to this exam datasheet the first time I took it because it ended up being more helpful than I gave it credit for. I will elaborate how I used this later on this blog
   
4. CBTNuggets PCNSA & PCNSE by Keith Barker: Since I did not do PCNSA or PCNSE (having only completed a PCCET) before they retired, I figured this would still be a good video series to knock out as part of my initial preparation. While I was able to knock out most of PCNSA, I only got through PCNSE partially before putting this course down in favor of the official Palo Alto Learning Platform. Regardless, these two courses were still helpful giving me exposure into high-level content idea for some of the NGFW Engineer topics as there was a fair amount of overlap in exam topic between PCNSA/PCNSE and new NGFW Engineer exam
   
5. **Udemy Course: Palo Alto Networks Next-Generation Firewall Engineer - Exams by Paweł Krakowiak**: I was initially skeptical of this resource because of the mixed reviews by many test takers had given that it did not adaquetly prepare you for the real exam. However, after failing it the first time, I purchased this practice exam course and to my surprise, it revealed big gap in 2 domains I had: SSL/TLS Profile (Certificate Profile, SSL Forward Proxy) & GlobalProtect
   
6. **[Wesley Cyber NGFW Engineer Playlist](https://www.youtube.com/playlist?list=PLltJsgfsuLOit54c49FkjTx2-51S5nVdI)**: Although this playlist is incomplete, I watched the first 3 videos prior to my first attempt and THOROUGHLY gone through the full playlist prior to my 2nd re-attempt. Given that Wes covered most of Domain 1: PAN-OS Networking Configuration, I rate his YouTube series highly valueable being able to watch him configure things hands on
7. INE Palo Alto Labs: This was more of an impulsive buy. I can't attest 100 percent that I needed it, but every little bit helps

## Background and initial preparation ##
Back in Jan 2025, I took (now-retired) Palo Alto Certified Cybersecurity Entry Level Technician (PCCET) as my entry point into the world of Palo Alto NGFW. While PCCET was no-where technical, I still appreciated the experience learning it. However, because [PCCET, PCNSA, and shortly-after PCNSE were retired](https://live.paloaltonetworks.com/t5/news/new-security-service-edge-engineer-certification-upcoming/ta-p/997555) in favor of role-based exams, I was not able to test myself against PCNSA content. After reviewing several of the new role-based certification as well as what online forums had to say about them, I determined that NGFW Engineer exam was the most appropriate exam to pursue given its scope. So I started preparation in November 2025

I started by watching CBTNuggets PCNSA and PCNSE course by Keith Barker to absorb in as much of the conceptual knowledge as I could. Because it was the winter season, I gave myself until Spring 2026 to prepare instead of relying on an aggressive approach to get it within 1 to 2 months because I did not want to go out during the winter season to take any exam and I want to take this one a bit more slowly. While I felt like I was initially going at a decent pace and was able to complete the PCNSA course, the sheer volume of content in PCNSE (almost double of PCNSA) I found to be too much so halfwaythrough PCNSE, I decided to drop it in favour of the learning from the official learning platform once January 2026 came around and I realized I needed to step up the pace.

I then opened the Palo Alto Learning (formerly known as Beacon) and continued forward, reviewing important high-level concept such as Interface Types, HA setup, Routing and Switching. This was where things got interesting as I started also gaining exposure to cloud NGFW concepts (VM-series, CN-series, Cloud Identity Engine, AI Runtime security, and many more), which completely blew me away because I was very unfamamiliar with a lot of it. Thankfully, because I had previously completed AZ-900 and AWS Cloud Practitioner, I was comfortable enough with many of the high-level cloud-specific concepts that Palo integrates with (such as Azure VNet, AWS VPC); only one I had no real understanding of was the Google Cloud. One thing I also want to note was that as I was going through the Palo Alto Learning platform, I was building my own Quizlet flashcard deck of concepts to review throughout the lifecycle of the exam. I thought this was important because it gave me a flashcard repository that I can periodically go through and casually review daily to ensure I remember the concepts that I learned via spaced repetition

## First Attempt ##
After I finished the Palo Alto learning course and first two video of WesleyCyber's NGFW playlist that he released, I (having committed to March 2026) went in for my first attempt into the exam, still not ensure what to expect of it. 

As I went through the exam, I can feel the unsettling motion going through my body. I felt so fuzzy answering many questions because many of which I would either knock down to 2 remaining answers and it would always come down to a 50-50 where I was just purely guessing. At the end I failed.

## Reviewing Exam Result and Determining next step ## 
While I'm not necessarily surprised at failing, I was still frustrated by the outcome and by the percentages that I got in my result. Frustrated, I went home and immediately pulled up the Exam Datasheet and copied it to a Google Docs. Then I commented on every single topic (listed on the subdomain) that I felt uncomfortable with.

I also impulsively bought an INE course (because it was on sale and had online Palo Alto Labs that I could use some extra practice in). I don't think this was a wise call, but my impulsiveness got the best of me and I was planning to pursue JNCIP - ENT later this year so I said I will make it worth it one way or another

Throughout my review session, I watched Wesleycyber's NGFW YouTube Series. Although the videos released only covered domain 1 at the time, I found it helpful to review it especially since I scored a 50 percent on Domain 1. Additionally, I started going through each of the Subdomain, locating appropriate Palo TechDocs for each topic that I deemed helpful. Soon after, I had a fully built out Exam Datasheet-based notes, marking important concepts that I needed to know in preparation for my re-take. I skipped Domain 3: Integration and Automation because I did the best on it on my first try (80 percent) and it was weighted the least (20 percent)

## Second Attempt ##
After reviewing everything, I went in for my 2nd attempt a month later, feeling much more confident about what I got wrong the first time. I confidently went through the questions, reading word for word to make sure I understand what I was being asked of. Thanks to the Exam Datasheet notes I took, I was able to pass it the 2nd go-round

## Advice to Others ##

**Understand CCNA-level knowledge, Security+, and Basic Cloud Concepts** : While the exam does not have any real pre-requisite, it demands a working (CCNA-level Networking knowledge), basic Security+ knowledge, and basic Cloud (Azure and AWS mostly) knowledge. Knowing how these work together in tandem with Palo Alto (especially concerning deploying VM-series Firewall) will increase your chances of success.
   



