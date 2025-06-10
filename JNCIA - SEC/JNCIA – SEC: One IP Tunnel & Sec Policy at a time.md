Continuing build onto Juniper Brigade after [JNCIA - Junos]( https://github.com/bobchen48/Writeups/blob/main/Juniper%20-%20Junos/Road%20to%20Junos.md?plain=1), I went into this exam hoping to achieve 2 objectives: Understand the inner workings of security policies, and learn how to configure VPN tunnels. 

## Why Security Policy and IPSec Tunnel ##
When I first encountered Security Policy, I had no idea what zones were and why zones exist. I was used to Security policies as static policies that traverse from one interface to another, never envisioned them tied to a logical zone.

In the same realm, when I was first shown a sample VPN Tunnel configuration, my mind was just blown. I had no idea what was going on in the configuration, let alone why there were so many lines. Although a colleague helped me to understand it a bit better, his, I still had more questions that needed to be answered.

Determined to understand both down to a science, I went into this certification determined that when I come out, I will hopefully get a better understanding of Juniper SRX offering.
## Resources Used ##
1. **Udemy Course Juniper JNCIA-SEC JN0-231 by S2 Academy**: The main video course used for this certification exam. Like S2 Academy’s video for JNCIA – Junos, I found this video course help break the objectives mentioned on JNCIA - SEC Blueprint objectives into digestible video courses that can be consumed easily.
  
2. **Juniper vLab – Security**: A virtual lab environment that provides a virtualized environment to test commands in configuration mode. For this exam, I used all the topology listed under Security as they provided setup relevant to the exam.
   
3. **JNCIA-Junos JN0-105 Practice Exams by S2 Academy**: Like JNCIA Junos Practice exam provided by S2 Academy I used when practicing for JNCIA Junos, I used this test bank as a complementary resource to S2 Academy's JNCIA Junos JN0-231. This provided me with 300+ practice questions that I can practice to test my understanding of exam content.
   
4. **Juniper Open Learning Portal – JNCIA – SEC**: I watched some of the lecture videos in this course (mostly when I first started studying for this exam, but similar to my JNCIA – Junos experience, I found this online portal course a bit redundant given I was already engulfed into the Udemy course. However, I made sure to take the practice exam at least to maximize my understanding of what I would be expecting on the actual exam.

## My Preparation - Some Thoughts ##
When I first started preparing for this exam, I had a basic, but scuffed understanding of address objects (logical objects that are used to represent an IP address). I witness a series of “set security policies from-zone trust to-zone untrust…” and I was left clueless, no idea what a “zone” was. In my head, I thought zone was a logical territory, but the question regarding what was inside a zone, remained. 


As I progress throughout this course, the concept of zone and IPSec Tunnel began to make sense as I started to understand why they exist and what purpose they serve in SRX devices. To me, zones was like territoritory (virtual) that contained a set of IP Adresses. Regardless though, once the idea of zones and their role in security policies cleared in my head, I began to understand why I was writing security policies the way I was writing it. It was a way to route packets the way I wanted them to be routed, based on a set of requirements.

Likewise, I recall first seeing 30+ lines of VPN tunnel and had no idea what was going on. What was st0 (it stands for security tunnel 0, a logical entity used to route traffic to a vpn tunnel). Once I started understanding the idea behind the command, they began to clarify in my brain and the rest was history.

<div align="center">
  <image src="[https://github.com/bchen96/Writeups/blob/main/Allied%20Solutions%20Internship/Big%20Questions.png](https://github.com/bobchen48/Writeups/blob/main/JNCIA%20-%20SEC/Route%20Based%20IPSec%20VPN%20-%20Part%201.jpg]">
</div>
<div align="center">
  <image src="[https://github.com/bchen96/Writeups/blob/main/Allied%20Solutions%20Internship/Big%20Questions.png](https://github.com/bobchen48/Writeups/blob/main/JNCIA%20-%20SEC/Route%20Based%20IPSec%20VPN%20-%20Part%201.jpg]">
</div>

## Advice to Others##
1.	**Understand Source NAT, Destination NAT, and Static NAT**: These three NAT are three of the most important components of security policies because they influence how packets are handled as it enters and exits SRX devices. Prior to this exam, I watched a Palo Alto Firewall YouTube regarding [NAT/Security Policy configuration] (https://www.youtube.com/watch?v=Ahrao6kBg8w) that clarified the consideration of NAT when configuring security policies
2.	**Getting into shape on Exam Date**: I did not really think hard about this in all my prior exam, but I started to notice that being in a really good shape both PHYSICALLY and MENTALLY can be a huge confidence booster by itself. Something I started doing more lately on exam date before an IT certification exam was eating chicken noodle soup ( breakfast or lunch). Chicken noodle soup that not only feels good when swallowed because of the rich broth, but it also does not feel “hard” on the body when consumed. This is important because on exam date, it’s important to avoid eating food that can negatively impact your digestive system. You want to ensure your body is in its best shape on exam date to increase your likelihood of passing the exam. 
