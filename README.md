Bizarre Actor Pouts On
======================

* [What did you call me!?](#what-did-you-call-me)
* [Get the facts!](#get-the-facts)
* [What does it all mean?](#what-does-it-all-mean)
* [How to](#how-to)



# What did you call me!? 
"Bizarre Actor Pouts On"... is a beautiful anagram for Anzu Robotics Raptor! Lets learn a little more about this bizarre actor, shall we? 

| ![I can haz Raptorburger?!](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/BizzareActorPouting.jpg) | 
|:--:| 
| *I can haz Raptorburger?!* |

The past few months have brought several announcements regarding a hot new White Labeled DJI powered product:

["Aloft Announces Strategic Partnership with Anzu Robotics to Launch the Raptor Drone, Elevating Enterprise Fleet Management and Airspace Compliance"](https://www.aloft.ai/blog/aloft-announces-strategic-partnership-with-anzu-robotics-to-launch-the-raptor-drone-elevating-enterprise-fleet-management-and-airspace-compliance/)

["Anzu Robotics has forged a strategic partnership with Aloft to power our airframes and ensure the security of your data"](https://www.anzurobotics.com/powered-by-aloft-air-control/)

["Whether you’re a prospective buyer, a current user, or just curious about what Anzu Robotics has to offer, you’ve come to the right place."](https://www.anzurobotics.com/faq/) 

Several statements have been made in an assertive fashion: 
```
WHAT IS THE RELATIONSHIP BETWEEN ANZU AND ALOFT?
Anzu Robotics and Aloft, formerly known as Kittyhawk, have forged a strategic partnership to bring to market quality and secure drone solutions. Anzu Robotics is responsible for each of its customers and their experience using the Raptor-series and any future Anzu Robotics products, however Anzu leverages Aloft’s development of their Air Control app for operation of the drone, storage of the data, and advanced features available in the enterprise version of the app.

WHERE DOES THE FIRMWARE ON THE RAPTOR-SERIES DRONES COME FROM?
When we finalized the licensing agreement we were provided a version of custom firmware as a snapshot in time. That firmware was then housed on Aloft’s servers for development and can’t be accessed or modified by anyone else. The flight dynamics of our drones were not redeveloped, so you’re getting world-class performance benefitting from more than a decade of aerial robotics R&D. We have taken the necessary measures to ensure that anything on our drones is void of data security vulnerabilities.

HOW ARE FIRMWARE UPDATES DONE ON THE RAPTOR-SERIES DRONES?
We do not anticipate forcing firmware updates unless they are absolutely critical for safety. We anticipate any firmware updates to be seldom, and would be done over the air from your controller. Additionally, no third-parties are able to force firmware updates through our system.
```

The statements have been further bolstered through third party commentary, and attestations: 

["White Knight Labs conducted a comprehensive penetration test on the Anzu Raptor, a cutting-edge drone platform developed by Aloft. The objective was to identify and mitigate potential security vulnerabilities, ensuring the drone's robust performance in real-world applications."](https://www.linkedin.com/posts/white-knight-labs_ensuring-the-security-of-the-anzu-raptor-activity-7201966025800572929-lUeW/)

["WKL Aloft Attestation Letter 05-22-2024"](https://www.anzurobotics.com/wp-content/uploads/2024/05/WKL-Aloft-Attestation-Letter-5-22-24-vFinal.pdf)

["Ensuring the Security of the Anzu Raptor: A Successful Penetration Test by White Knight Labs"](https://www.aloft.ai/blog/ensuring-the-security-of-the-anzu-raptor-a-successful-penetration-test-by-white-knight-labs/)

# Get the facts! 
The Aloft AWS bucket was raided by unknown individuals, as well as security researchers alike. This occured before WKL completed their testing. It is alleged that this misstep was mitigated after the WKF report was in hand. 

[Pre WKL Audit AWS - DJI CDN dump](https://archive.org/details/anzu-quick-analysis)

["Anzu Raptor Drone, RC and App A quick analysis"](https://think-awesome.com/Anzu_quick_analysis.pdf)

From the report above a very important observation is made: 
"I was able to check the DJI server for the firmware, same as DJI Assistant 2 tool one can manually download firmware for updates. Let’s see if we download the 0802 firmware from DJI directly, click this link and see what you get"
[wm265e_0802_v20.00.00.07_20231212.pro.fw.sig](https://archive.org/download/anzu-quick-analysis/Users/kfinisterre/Desktop/Aloft_DJI-CDN_dump/wm265e_0802_v11.07.01.16_20240625.pro.fw.sig) 

"There is our Anzu firmware living on the DJI CDN, so the firmware is also hosted by DJI in contrary to the claims from Anzu."

We previously learned "Aloft is ISO 27001 and SOC 2 Type II certified", because I'm lazy I asked ChatGPT the following question: 

| ![GPTAintWrong](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/GPTAintWrong.png) | 
|:--:| 
| *GPTAintWrong* |

I don't disagree with the answer


# What does it all mean? 

Welp the firmware was leaked, and we weren't the only ones to get it... 
| ![others.jpg](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/others.png) | 
|:--:| 
| *others* |

This means you can make your own DIY Raptor using the [DJI Slack OG tools](https://github.com/o-gs/dji-firmware-tools) 

| ![1.jpg](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/1.jpg) | 
|:--:| 
| *Stock M3 with Anzu branded Aloft software* |

| ![2.jpg](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/2.jpg) | 
|:--:| 
| *DIY M3 showing video feed in Anzu flavored Aloft Aircontrol* |

| ![3.jpg](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/3.jpg) | 
|:--:| 
| *App auto updated to 1.12.22.119* |

| ![4.jpg](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/4.jpg) | 
|:--:| 
| *Warranty repair uses these serial numbers... lol* |

# How to
IF you are lucky an [OG](https://www.dji-rev.com) may help you out. You probably need to hit #spoon-feeding however. 

See the retroroms ["List of the Modules and What they Effect"](https://github.com/MAVProxyUser/BizarreActorPoutsOn/tree/main) for more detail. 



