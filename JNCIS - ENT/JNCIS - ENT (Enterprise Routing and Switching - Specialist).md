# JNCIS - ENT - Lesson on Resilience and Bouncing back from Failure #

On 9-8-2025, I was able to accomplish the JNCIS-ENT (Juniper Enterprise Routing and Switching, Specialist) Exam. Accomplishing this one to meant more than just anoter certification because this one taught me the importance of being resilient and bouncing back from failure.

## Resources Used ##
1. **Udemy Course Juniper Networks JNCIS-ENT Certification: Master the Essentials by Ben Jacobson**: This was my main video course I used to prepare for this certification. Looking back, I felt like this course was not very helpful in contributing to my preparation for the exam. I wished I used CBTNuggets course that was available instead. I was drawn to this course originally because it was only 12 hours long, but shorter doesn't always mean better
2. **Juniper Open Learning JNCIS-ENT**: I initially paired this as a supplemental to my Udemy course, but looking back, this course was the reason that likely helped me passed the exam as it taught many of the content that were missed entirely or covered very briefly in the Udemy course
3. **Udemy Course: Juniper JNCIS-ENT (JN0-351) - Practice Exam by Nerd Exams**: Like my previous Juniper Exams (Junos and JNCIA - SEC), I used Nerd Exams JNCIS-ENT Exam prep). This combined with the practice questions on Juniper Open Learning was enough practice questions to prepare me.

## Preamble - Reflection on Failed VCF ##
Back around June to July 2025 after passing my [JNCIA - SEC](https://github.com/bobchen48/Writeups/blob/main/JNCIA%20-%20SEC/JNCIA%20-%20SEC%3A%20My%20Certification%20Journey.md), I felt immense confidence while preparing for VMware Cloud Foundation - Administrator (5.2) Exam that I was going to crush it in July. However, I was knocked down to reality as my [exam score showed a FAIL](https://github.com/bobchen48/Writeups/blob/main/VCP%20-%20VCF%20(VMware%20Cloud%20Foundation)%205.2/VCP-VCF.md). I remember leaving from the exam to go to the store, then walking home that afternoon, feeling down realizing that I was NOT invincible to failing. As bad as it was, I knew in the back of my mind that the only way to grow was to embrace the failures that came along the way (while still acknowledging the immediate pain of failure).

## Initial Preparation ##
Many of the r/juniper subreddit I was reading through when casually scoping out the difficulty of the exam compared exam difficulty of CCNA. Given I passed CCNA, I was not too afraid to tackle this exam, though the self-doubt after failing my VCF haunted me as I was afraid I could be at the risk of failing this. Given this, I did not want to "assume" I knew the content. As such, I went exploring for courses.

When I was browsing Udemy for video courses for JNCIS-ENT, the one (and only video course) that came up was Ben Jacobson's JNCIS-ENT course. Naturally, I bought it without a second guess and I began consuming the content.

## Midway Study - Feelings of Content Emptiness ##
After going through Ben Jacobson's Udemy course, I thought to myself "That's it??? No way that was all I needed to know". My gut was telling me I needed a second pass (from a different source) as I felt so many topics I learned were skimmed at surface level relative to what I believe was on exam objective. As a result, I obtained the JNCIS-ENT course on Juniper's Open Learning Portal (Free by the way) and went through it from start to finish. Feeling validated by my hunch, I felt satisified that the Open Learning Portal course covered gaps that were either missing or skimmed over in Ben Jacobson's course.

After consuming both course, I started practicing using practice questions I bought from Udemy (by Nerd Exams) and 40-question from Juniper Open Portal (It got intense in the final 2 days and night before leading up)

## Exam and Post-Exam ##
On the night before the exam, I was having difficulty sleeping as I was bewildered by the thought of failing again after my VCF failure. I sat there in bed thinking "am I gonna be able to do this?, What will happen if I fail again? etc".

Come morning, I eat some Chicken Noodle soup and go to my test center. I remember the first 20 questions, I was flying through it with confidence, knocking out 25 questions in only 15 minutes (while flagging only those I have very slight doubt in that I felt needed a second look). Feeling like I was going too fast, especially considering I had 90 minutes to go through 65 questions, I took a short pause and carefully read through my next 20 questions (and the choices presented) ensuring that I understood what was being asked.

At the end of the exam after reviewing my answer choices, I took a deep breath, nervously pressing "End Review" as I was ready to accept my fate (to fail). To my relief, I was met with a pass. I left the test center feeling accomplished and bounced back.

## Final Thoughts - Cisco vs Juniper STP Port cost calculation##
One interesting topic I learned throughout the lifecycle of preparing for this exam was analyzing the difference between Cisco and Juniper's methodology in _Spanning Tree Port cost calculation_ (image below). I remember sharing with a coworker (who also passed CCNA) how "stupid" Cisco's STP default port cost calculation was compared to Juniper (seen below). Cisco sets "seemingly" arbitary values (2, 4, 19, 100 for their respective ports) whereas Juniper uses multipliers of 10 in cost (starting at 2000) as you multiply the speed of the port by 10; a more systematic approach.


<div align="center">
  <image src="https://github.com/bobchen48/Writeups/blob/main/JNCIS%20-%20ENT/Cisco%20default%20STP%20port%20cost.png">
</div>

<div align="center">
  <image src="https://github.com/bobchen48/Writeups/blob/main/JNCIS%20-%20ENT/Juniper%20default%20STP%20port%20cost.jpg">
</div>





