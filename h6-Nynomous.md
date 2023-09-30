# Summarise: 7 Things You Should Know About Tor
The article discusses seven key things that individuals should know about Tor, a privacy-focused network known for providing anonymity online.

1. Tor Still Works: Despite NSA revelations about attempts to compromise it, Tor remains an effective tool for online anonymity. While certain users have been compromised through exploits or misconfigurations, the core cryptographic protection of Tor appears to remain intact. However, it cannot prevent monitoring if both ends of the communication are actively surveilled.

2. Tor is Not Only Used by Criminals: A common misconception is that Tor is exclusively used by criminals and pedophiles. In reality, Tor serves various purposes, including circumventing censorship, secure military communications, protecting families, aiding journalists, and more. It can even help users protect against criminal tactics like identity theft.

3. Tor Does Not Have a Military Backdoor: Although initially funded by the US Navy, Tor's code has been scrutinized by security experts and cryptographers, confirming there is no hidden military backdoor. It is an open-source project developed by privacy and anonymity-focused activists.

4. No One in the US Has Been Prosecuted For Running a Tor Relay: As per the Electronic Frontier Foundation (EFF), no one in the US has faced prosecution for running a Tor relay. While running an exit relay may attract law enforcement attention, EFF believes that running a relay is generally not illegal in the United States. However, engaging in criminal activities through Tor may lead to legal consequences.

5. Tor is Easy to Use: Contrary to the perception that privacy software is complex, Tor offers user-friendly options like the Tor Browser Bundle, preconfigured for secure Tor usage. Tails, a live operating system that routes all internet traffic through Tor, is another easy-to-use option.

6. Tor is Not as Slow as You Think: Although Tor may be slower than regular internet connections, ongoing efforts by Tor developers aim to enhance its speed. Expanding the network by creating more relays is one way to contribute to improving its speed.

7. Tor is Not Foolproof: Tor's effectiveness depends on correct usage. Users should stick to recommended tools like the Tor Browser Bundle or Tails and keep their software up to date. Logging into services like Google and Facebook via Tor may still allow these services to view your communications within their systems. Additionally, adversaries with access to both sides of the connection could potentially perform statistical analysis to identify the user.

In conclusion, Tor remains a robust anonymity tool, dispelling misconceptions that it is exclusively for criminals or has military backdoors. It offers user-friendly options, is continually improving in speed, and, while not foolproof, provides strong anonymity when used correctly. Educating the public about Tor's capabilities can help individuals take back their online privacy.

### https://www.eff.org/deeplinks/2014/07/7-things-you-should-know-about-tor


# Summarise: Shavers & Bair 2016: Hiding Behind the Keyboard: The Tor Browser

The article introduces "The Onion Router" browser, commonly known as Tor, which is designed for anonymous internet use. Tor is essentially a modified version of the Firefox browser that conceals a user's IP address, making it extremely challenging to trace or identify them. It offers a combination of ease of use and effective anonymity, making it accessible to nearly anyone.

Tor's primary purpose is to enable unfettered and anonymous internet communication. It allows users to access blocked websites, facilitates anonymous communication for whistleblowers, and ensures privacy for legitimate business and personal conversations. Despite its origins as a project funded by the US government, Tor is now a decentralized and open-source network, continually improved by a global community of privacy-focused experts.

The article presents two perspectives for examining Tor: one as a forensic tool to analyze devices with Tor artifacts and another as an ongoing investigation to defeat Tor for capturing communications or identifying users. Tor works by routing internet traffic through random relays and encrypting data at each step, making it highly secure and difficult to trace.

Key points about Tor:

1. How Tor Works: Tor routes internet traffic through a series of relays, each stripping a layer of encryption until it reaches its final destination. The random selection of relays changes every 10 minutes, enhancing anonymity.

2.Tor Nodes: The Tor network relies on volunteer-run relays, making it challenging to pinpoint users. There are also "bridges" that are not publicly listed, making them difficult to block.

3.User-Friendly: The Tor browser is user-friendly, similar to Firefox. Downloading and configuring it typically takes only about 10 minutes, making it accessible to most users.

4.Illicit Use: While Tor offers strong anonymity, it can also be used for illegal activities, including criminal communication and file sharing. It poses challenges for law enforcement to track and apprehend suspects.

5.Forensic Analysis: Investigating Tor involves examining devices with Tor artifacts or attempting to defeat Tor for active investigations. However, both tasks are exceptionally difficult due to Tor's design.

In summary, Tor is a powerful tool for online anonymity, with legitimate and illicit applications. It provides a high level of privacy but also presents significant challenges for investigators and forensic analysts due to its robust security features. Understanding how Tor works is crucial for both defenders of privacy and law enforcement agencies seeking to combat illicit activities conducted through the network.

For the chapter of Tracking Criminals Using TOR it discusses the challenges of tracking criminals who use the Tor network for anonymity and outlines various methods and instances where Tor users have been identified by law enforcement.

1. Difficulty in Tracking Tor Users: Tracking Tor users is notoriously difficult due to the network's design, which prioritizes anonymity. Government agencies around the world are actively working on deanonymizing Tor to locate criminals and terrorists.

2. Limited Successes: While there have been a few high-profile cases where law enforcement successfully deanonymized Tor users, these successes are often the result of errors made by the suspects rather than breaking Tor's security.

3 .FBI's Exploit: An example is the FBI's takedown of a child pornography hosting service. They exploited a vulnerability in Firefox (CVE-2013-1690) to capture the true IP addresses of Tor users who visited criminal websites. This exploit was successful due to a bug in the Tor Browser Bundle.

4. User Errors: One of the major weaknesses of the Tor browser is user customization. Altering settings or allowing certain website features can leak information and compromise anonymity. For example, allowing geolocation or running certain scripts can reveal the user's true IP address.

5. Ongoing Research: Researchers have been studying Tor for vulnerabilities and methods to deanonymize users for years. Some theories involve attacking the Tor network itself or gaining control of entry and exit nodes to correlate traffic and identify users.

6 .Man-in-the-Middle Attacks: Nation-states and well-funded entities can attempt man-in-the-middle attacks to intercept Tor traffic. However, compromising Tor remains challenging even for them.

7. Tracking IP Addresses: Obtaining the true IP address of a Tor user is a common investigative goal. Law enforcement may use methods such as embedding tracking codes in emails or documents sent to suspects. When the suspect opens the document or email, the tracking code can capture their IP address.

8. Identifying Tor Users on Corporate Networks: In cases involving internal corporate networks, network administrators may identify Tor users if the network is being used with Tor. This can be valuable for investigations, as it allows authorities to correlate network access times with threatening emails or other activities.

9. Breaks in Cases: Many cases are solved due to mistakes made by suspects. For instance, a suspect might unintentionally use a non-Tor browser, revealing their true IP address when communicating with victims.

It emphasizes that while Tor provides strong anonymity, mistakes made by users and potential errors in their usage can lead to the identification of Tor users. These cases highlight the delicate balance between privacy and law enforcement's efforts to combat criminal activities conducted through the network.

### https://learning.oreilly.com/library/view/hiding-behind-the/9780128033524/

