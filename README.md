"Bizarre Actor Pouts On"... is a beautiful anagram for Anzu Robotics Raptor! Lets learn a little more about this bizarre actor, shall we? 

![I can haz Raptorburger?!](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/BizzareActorPouting.jpg)

["Aloft Announces Strategic Partnership with Anzu Robotics to Launch the Raptor Drone, Elevating Enterprise Fleet Management and Airspace Compliance"](https://www.aloft.ai/blog/aloft-announces-strategic-partnership-with-anzu-robotics-to-launch-the-raptor-drone-elevating-enterprise-fleet-management-and-airspace-compliance/)

["Anzu Robotics has forged a strategic partnership with Aloft to power our airframes and ensure the security of your data"](https://www.anzurobotics.com/powered-by-aloft-air-control/)

["Whether you’re a prospective buyer, a current user, or just curious about what Anzu Robotics has to offer, you’ve come to the right place."](https://www.anzurobotics.com/faq/) 

WHAT IS THE RELATIONSHIP BETWEEN ANZU AND ALOFT?
Anzu Robotics and Aloft, formerly known as Kittyhawk, have forged a strategic partnership to bring to market quality and secure drone solutions. Anzu Robotics is responsible for each of its customers and their experience using the Raptor-series and any future Anzu Robotics products, however Anzu leverages Aloft’s development of their Air Control app for operation of the drone, storage of the data, and advanced features available in the enterprise version of the app.

WHERE DOES THE FIRMWARE ON THE RAPTOR-SERIES DRONES COME FROM?
When we finalized the licensing agreement we were provided a version of custom firmware as a snapshot in time. That firmware was then housed on Aloft’s servers for development and can’t be accessed or modified by anyone else. The flight dynamics of our drones were not redeveloped, so you’re getting world-class performance benefitting from more than a decade of aerial robotics R&D. We have taken the necessary measures to ensure that anything on our drones is void of data security vulnerabilities.

HOW ARE FIRMWARE UPDATES DONE ON THE RAPTOR-SERIES DRONES?
We do not anticipate forcing firmware updates unless they are absolutely critical for safety. We anticipate any firmware updates to be seldom, and would be done over the air from your controller. Additionally, no third-parties are able to force firmware updates through our system.

["White Knight Labs conducted a comprehensive penetration test on the Anzu Raptor, a cutting-edge drone platform developed by Aloft. The objective was to identify and mitigate potential security vulnerabilities, ensuring the drone's robust performance in real-world applications."](https://www.linkedin.com/posts/white-knight-labs_ensuring-the-security-of-the-anzu-raptor-activity-7201966025800572929-lUeW/)

["Ensuring the Security of the Anzu Raptor: A Successful Penetration Test by White Knight Labs"](https://www.aloft.ai/blog/ensuring-the-security-of-the-anzu-raptor-a-successful-penetration-test-by-white-knight-labs/)

(Pre WKL Audit AWS / DJI CDN dump](https://archive.org/details/anzu-quick-analysis)

["Anzu Raptor Drone, RC and App A quick analysis"](https://think-awesome.com/Anzu_quick_analysis.pdf)

"Let’s check: I was able to check the DJI server for the firmware, same as DJI Assistant 2 tool one can manually download firmware for updates. Let’s see if we download the 0802 firmware from DJI directly, click this link and see what you get:"
[wm265e_0802_v20.00.00.07_20231212.pro.fw.sig](https://archive.org/download/anzu-quick-analysis/Users/kfinisterre/Desktop/Aloft_DJI-CDN_dump/wm265e_0802_v11.07.01.16_20240625.pro.fw.sig) "Correct: There is our Anzu firmware living on the DJI CDN, so the firmware is also hosted by DJI in contrary to the claims from Anzu."

We previously learned "Aloft is ISO 27001 and SOC 2 Type II certified", because I'm lazy I asked ChatGPT the following question: 

"Given that Aloft is ISO 27001 and SOC 2 Type II certified, it would be unexpected and concerning if they had an open AWS share exposing development software and firmware. Both ISO 27001 and SOC 2 Type II certifications indicate a strong commitment to information security and data protection, including strict controls over access to sensitive data and secure handling of development assets."

I don't disagree with the answer: 

"Open AWS Share Exposing Development Software and Firmware:
ISO 27001: This standard requires organizations to establish, implement, maintain, and continually improve an information security management system (ISMS). This includes strict access control mechanisms and regular risk assessments to identify and mitigate security vulnerabilities.
SOC 2 Type II: This certification focuses on the operational effectiveness of an organization's security controls over a period of time. It covers aspects such as confidentiality, privacy, and security, emphasizing robust access control and data protection measures.
Given these certifications, an open AWS share exposing development software and firmware would indicate a significant lapse in security practices and controls, potentially violating the standards and principles underlying their certifications.

Control of Encryption Keys for White-Labeled Software:
It is generally expected that a company in control of encryption keys for software, especially if they white-label products, maintains stringent security practices. Control over encryption keys is crucial for ensuring the integrity, confidentiality, and authenticity of the software deployed on hardware.
Both ISO 27001 and SOC 2 Type II frameworks emphasize the importance of managing and securing cryptographic keys. These keys should be safeguarded against unauthorized access and misuse, often through mechanisms like hardware security modules (HSMs) or key management services (KMS).
If Aloft were to adhere strictly to the security principles mandated by their certifications, they would be expected to maintain rigorous control over encryption keys and ensure secure storage and handling of all sensitive assets, including development software and firmware."

