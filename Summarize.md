# Summarize the episode of Jason's Pen Test on Darknet Diaries Podcast

For the Darkness Diaries Boardcast I chose Episode 130: Jason’s Pen Test, As Jason is a penetration tester he is sharing many of stories while at work that he breaks into buildings and computers, and talks about the time he discovered a major security flaw in a popular mobile banking app. The topic is interesting and banking app are almost everyone’s daily based tools. I really wanted to know about the information behind this. Besides,  I found it’s always easier to start a study or something new by listening interesting stories. 

The episode starts by a story happened in the garage, the accident made Jason successfully parked into management parking lot. Which reminds me many leak were happened when there’s an accident. And then it introduced how he found  darknet fourm called SahdowCrew to self learning how to make fake ID. Although he didn't sell many fake IDs, he was passionate about perfecting his skills. However, the Secret Service shut down ShadowCrew, leading to panic among its members, including Jason. Worried about potential legal consequences, Jason hastily disposed of his fake ID materials while being pulled over by a cop, narrowly avoiding discovery.

The incident made Jason quit the fake ID business due to the fear of getting caught. He transitioned into a legitimate career in computer security, initially fixing computers and then becoming a penetration tester. He worked for HP, conducting penetration tests on various companies to assess their security. His role included breaking into networks to identify vulnerabilities, particularly in the context of PCI compliance for credit card processing.

Jason's expertise focused on network hacking, and he recounted a humorous story of a physical penetration test where his familiarity with a previous employer's security measures allowed him to easily break in during a subsequent test. These part was how Jason's journey from making fake IDs to transitioning into a legitimate career in cybersecurity as a penetration tester.

And then Jason discusses the experiences  of penetration testing, particularly focusing on physical and mobile application penetration testing. In one instance, Jason needed to breach a door with a magnetic lock that unlocked when someone approached from the inside. He used a deflated blow-up doll, inflated it on the other side of the door to trigger the lock, and gained access to the premises. Another assignment involved breaking into a secure server room by climbing through ceiling tiles. Despite a mishap where he fell through the ceiling, he achieved his objective.

Shifting to mobile app penetration testing, Jason explored a bank's mobile banking app, which featured a check deposit feature via photos. He engaged in reconnaissance by identifying the bank's publicly exposed web servers and scrutinizing their applications. Jason then focused on the check deposit functionality, capturing traffic between the app and servers to understand the process better.

It highlights the unconventional and creative approaches penetration testers use to assess security vulnerabilities in physical environments and mobile applications, shedding light on their crucial role in identifying potential weaknesses.He uses a proxy tool called Burp Suite to intercept web traffic between the website and his browser. He analyses the process of uploading check images to the website's API, which then stores them in an AWS storage bucket. The surprising discovery is that this AWS bucket is open and accessible by anyone. Jason identifies sensitive information, such as names, addresses, account numbers, and transaction history for users of the check deposit feature, revealing a significant privacy breach. This information is new to me and we are starting to learn AWS just right now. But of course, Jason said it was on the younger age of the AWS. 

Moving on to the security testing of a different site, Jason examines a naughty website that offers live cams and content related staff. He creates a user account and investigates the password policy, finding that the site requires a minimum five-character password without special characters or numbers. Additionally, he discovers a flaw in the password reset process. By initiating password resets for a targeted account, he identifies that the site generates and sends five-character passwords, which he can brute-force within fifteen minutes due to the weak policy. Through this method, he gains unauthorized access to the account and achieves the test's objective.

Jason also discusses his penetration testing experience on that website. He explains how he used Burp Suite's Intruder tool to perform a brute-force attack on password resets, gaining unauthorized access to user accounts due to weak password policies. He highlights the issues with content sites opting for weaker password complexity to reduce user friction, leading to security vulnerabilities.

Additionally, Jason explores further security flaws on the website. He details how he found cross-site scripting (XSS) vulnerabilities and a way to access paid streams without payment. The website also facilitated user interactions and allowed connections between users, which drew parallels to the Ashley Madison scandal involving a data breach of a website for extramarital affairs.

Jason reflects on how he may have prevented a potential breach similar to Ashley Madison's by identifying and addressing security problems on the site he tested. The conversation touches on the perspective of young Jason, engaging in less ethical hacking activities, and how his current experience as a professional penetration tester gives him a greater appreciation for the significance and impact of his work.

## Reference https://darknetdiaries.com/episode/130/


# Summarize Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains

Intelligence-driven computer network defense is essential due to advanced persistent threats (APTs). Traditional vulnerability-focused approaches are insufficient against APTs, necessitating a deep understanding of the threat's intent, capabilities, patterns, and doctrine. The intrusion kill chain offers a structured analysis of intrusions, aiding in identifying indicators and guiding defensive actions. This approach prioritizes addressing capability gaps and evaluating defender effectiveness.

By incorporating threat awareness into resilience building against APTs, defenders can turn adversary persistence into a liability, reducing their success chances. The kill chain highlights an asymmetry where repeated aggressor components become liabilities. Analyzing repetition's nature for specific adversaries, whether for convenience or other reasons, involves assessing costs. Balancing intruders' cost-benefit ratio is crucial, indicating information superiority. Models of information superiority could inform attack and exploitation doctrine development.

The paper introduces an intrusion kill chain model in computer espionage, acknowledging broader implications beyond this context. This research intersects with disciplines like IED countermeasures, emphasizing the significance of intelligence-driven defense against evolving cyber threats.

Intelligence-Driven Computer Network Defense, informed by analysis of adversary campaigns and intrusion kill chains, is a proactive cybersecurity approach that focuses on understanding and countering advanced cyber threats. This strategy combines threat intelligence, analysis of historical attack patterns, and a deep comprehension of an attacker's tactics, techniques, and procedures (TTPs) to enhance the security posture of computer networks.

Intelligence-driven signifies the emphasis on collecting and analyzing threat intelligence to gain insights into the methods and motivations of cyber adversaries. By studying their previous campaigns, tools, infrastructure, and behaviors, defenders can anticipate potential attack vectors and vulnerabilities that attackers might exploit.

The concept of  adversary campaigns  refers to the orchestrated series of attacks carried out by cybercriminals or threat actors. By comprehensively analyzing these campaigns, security teams can discern commonalities, trends, and evolving strategies employed by adversaries. This knowledge helps in creating more effective defensive measures and anticipating future attacks.

Kill chains refer to the stages an attacker goes through during a cyber intrusion, from the initial reconnaissance to the final exfiltration of data. Analyzing these kill chains allows defenders to map out an attacker's path and identify potential points of disruption or prevention. It aids in recognizing early indicators of compromise and blocking attackers at various stages of their operation.

It involves continuous monitoring, threat detection, incident response, and mitigation strategies that align with the insights gained from threat intelligence and analysis of adversary campaigns and intrusion kill chains. By proactively adapting defenses based on evolving threat landscapes, organizations can better anticipate and counter sophisticated cyber threats, reducing their risk exposure and enhancing their overall cybersecurity posture.

## Reference https://lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Intel-Driven-Defense.pdf


# Install Debian

I have teied many times in my laptop, but it's always shows Error caused by signal 9. I have followed all correct steps on the instrctions and also searched for the solutions but non of them works. As a Mac user I am going to try QEMU that tearch has recommand. 

Tried UTM with ARM64

<img width="975" alt="Screenshot 2023-08-26 at 18 12 00" src=<img width="902" alt="Screenshot 2023-08-28 at 10 05 30" src="https://github.com/bga651/Information-Security/assets/114089466/c590e104-9fd0-40d6-9cda-84e9b3a56135">
<img width="900" alt="Screenshot 2023-08-28 at 10 05 44" src="https://github.com/bga651/Information-Security/assets/114089466/6814e255-395f-4a74-a531-8abfbe9155de">
<img width="808" alt="Screenshot 2023-08-28 at 10 05 58" src="https://github.com/bga651/Information-Security/assets/114089466/c00fe6a2-65ca-49b4-a50f-af4ed841aed6">
<img width="876" alt="Screenshot 2023-08-28 at 10 18 13" src="https://github.com/bga651/Information-Security/assets/114089466/50ef5bed-943e-48ee-956c-9e6f622c0b60">
<img width="616" alt="Screenshot 2023-08-28 at 10 28 16" src="https://github.com/bga651/Information-Security/assets/114089466/c09bd2d8-ea89-4f06-89d6-8a4b1178b9be">
<img width="885" alt="Screenshot 2023-08-28 at 11 53 23" src="https://github.com/bga651/Information-Security/assets/114089466/72d6fe3d-7817-494c-acbb-bb5ca5a996e4">
<img width="757" alt="Screenshot 2023-08-28 at 11 53 43" src="https://github.com/bga651/Information-Security/assets/114089466/553d313f-0600-451a-a2b6-8174d5ad1f05">
<img width="792" alt="Screenshot 2023-08-28 at 12 02 01" src="https://github.com/bga651/Information-Security/assets/114089466/fb7b2e15-607e-41c8-956f-3e32065bf766">
<img width="1279" alt="Screenshot 2023-08-28 at 12 02 15" src="https://github.com/bga651/Information-Security/assets/114089466/fe117e33-eaf2-4735-aa13-1308fd39af45">
<img width="1283" alt="Screenshot 2023-08-28 at 12 04 27" src="https://github.com/bga651/Information-Security/assets/114089466/85d3e9fb-77d0-4e9f-8042-0a0701d710a0">
<img width="1269" alt="Screenshot 2023-08-28 at 12 09 23" src="https://github.com/bga651/Information-Security/assets/114089466/9e7a1dc7-437c-427e-b684-8fd6b2eed629">
<img width="1286" alt="Screenshot 2023-08-28 at 12 09 36" src="https://github.com/bga651/Information-Security/assets/114089466/059da30b-cefb-4510-b8ec-dd8ff5e469a8">
<img width="1275" alt="Screenshot 2023-09-02 at 18 47 17" src="https://github.com/bga651/Information-Security/assets/114089466/5d4b6ade-cfbe-42b4-82ed-8422bdec23db">
<img width="1279" alt="Screenshot 2023-09-02 at 18 57 19" src="https://github.com/bga651/Information-Security/assets/114089466/b78e624f-2794-479a-8695-de3f079fadc6">
<img width="782" alt="Screenshot 2023-09-02 at 18 59 35" src="https://github.com/bga651/Information-Security/assets/114089466/197e2397-efd0-486d-aa61-4e8f51ef6a9c">
"https://github.com/bga651/Information-Security/assets/114089466/d6ec15fa-ea53-460e-bc76-922d2c1a356b">




