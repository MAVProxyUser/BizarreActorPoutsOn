Bizarre Actor Pouts On
======================

* [What did you call me!?](#what-did-you-call-me)
* [Get the facts!](#get-the-facts)
* [What does it all mean?](#what-does-it-all-mean)
* [How to](#how-to)
* [Mitigation](#mitigation)


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
[wm265e_0802_v20.00.00.07_20231212.pro.fw.sig](https://archive.org/download/anzu-quick-analysis/Users/SlackOG/Desktop/Aloft_DJI-CDN_dump/wm265e_0802_v11.07.01.16_20240625.pro.fw.sig) 

"There is our Anzu firmware living on the DJI CDN, so the firmware is also hosted by DJI in contrary to the claims from Anzu."

We previously learned "Aloft is ISO 27001 and SOC 2 Type II certified", because I'm lazy I asked ChatGPT the following question: 

| ![GPTAintWrong](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/GPTAintWrong.png) | 
|:--:| 
| *GPTAintWrong* |

I don't disagree with the answer


# What does it all mean? 
Very specifically it calls into question the statements that indicate Aloft / Anzu Raptor firmware "can’t be accessed or modified by anyone else", and that "no third-parties are able to force firmware updates through our system" 

Welp the firmware was leaked, and we weren't the only ones to get it... so the first statement is already confirmed as being false 1) because it was on DJI Content Delivery Network, 2) because it was leaked via AWS.
| ![others.jpg](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/others.png) | 
|:--:| 
| *Those before us? or those shoulder to shoulder with us?* |

This means you can make your own DIY Raptor using the [DJI Slack OG tools](https://github.com/o-gs/dji-firmware-tools), which brings the second statement on the ability to "force firmware updates" into question. Anyone with physical access to a raptor can technically force a firmware update. At any step in the supply chain, anyone with DJI firmware keys can additionally modify the firmware. Flashing can be done by anyone with the correct tools of course. 

Photos below donated by OG bin4ry:<br>
https://www.linkedin.com/in/makrisandreas/<br>
https://x.com/Bin4ryDigit

| ![1.jpg](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/1.jpg) | 
|:--:| 
| *Stock M3T with Anzu branded Aloft software* |

| ![2.jpg](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/2.jpg) | 
|:--:| 
| *DIY M3T showing video feed in Anzu flavored Aloft Aircontrol* |

| ![3.jpg](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/3.jpg) | 
|:--:| 
| *App auto updated to 1.12.22.119* |

| ![4.jpg](https://github.com/MAVProxyUser/BizarreActorPoutsOn/raw/main/4.jpg) | 
|:--:| 
| *Warranty repair uses these serial numbers... lol* |

["So here we go on the brink of a DJI ban. Is our knight in shining armor Anzu Robotics? So I have to ask, Randall Warnas can you retro an existing DJI aircraft to make it NDAA compliant? asking for a friend..."](https://www.linkedin.com/posts/andreas-aj-johansson-28334b51_dji-uas-drones-activity-7206867058356068352-3aKn/?utm_source=share&utm_medium=member_desktop)
It won't be NDAA compliant, but sure, knock yourself out... go on and retrofit your DJI Mavic 3 series controller with Aloft Air Control for Raptor, and flash the firmware to match the original Raptor firmware. Have fun! 

# How to
*coming soon*

We have determined the Raptor firmware to be nearly identical to DJI M3E/M3T update from 2023-12-28 aka [v09.00.05.05](https://forum.dji.com/forum.php?mod=viewthread&tid=304298)
[https://web.archive.org/web/20240120220229/https://enterprise.dji.com/mavic-3-enterprise/downloads](https://web.archive.org/web/20240120220229/https://enterprise.dji.com/mavic-3-enterprise/downloads)

[DJI Mavic 3 Enterprise Mavic 3E DJI Pilot Offline Firmware Update v09.00.05.05 - 2023-12-28](https://terra-1-g.djicdn.com/b20074248eff4b7f957d0f1a5ab29253/firmware/御3行业版/M3T_UAV_09.00.05.05_pro.zip)

[DJI Mavic 3 Enterprise Mavic 3T DJI Pilot Offline Firmware Update v09.00.05.05 - 2023-12-28](https://terra-1-g.djicdn.com/b20074248eff4b7f957d0f1a5ab29253/firmware/御3行业版/M3E_UAV_09.00.05.05_pro.zip)

[Archive.org retro DJI M3 Enterprise downloads page](https://web.archive.org/web/20240120220229/https://enterprise.dji.com/mavic-3-enterprise/downloads)

You can compare the software functionality vs the known [Eratta](https://dl.djicdn.com/downloads/DJI_Mavic_3_Enterprise/20230829/DJI_Mavic_3E_3T_Known_Issue_List_EN.pdf) list as well. 

Software date breakdown 
```
+---------+-------------------+------------+------------------+------------+------------------+------------+------------------+------------+
| Module  | wm265e            | Date       | wm265e           | Date       | wm265t           | Date       | wm265t           | Date       |
| ID      | (20.00.0005)      |            | (09.00.0505)     |            | (20.00.0005)     |            | (09.00.0505)     |            |
+---------+-------------------+------------+------------------+------------+------------------+------------+------------------+------------+
| 0802    | WM265E_E2         | 2023-12-12 | WM265E_E2        | 2023-12-22 | WM265T_E2        | 2023-12-12 | WM265T_E2        | 2023-12-22 |
| 1502    | WM265_E1E         | 2023-12-12 | WM265_E1E        | 2023-12-22 | WM265_E1E        | 2023-12-12 | WM265_E1E        | 2023-12-22 |
| 1100    | Battery           | 2023-07-31 | Battery          | 2023-07-31 | Battery          | 2023-07-31 | Battery          | 2023-07-31 |
| 1200    | ESC_0             | 2022-12-08 | ESC_0            | 2022-12-08 | ESC_0            | 2022-12-08 | ESC_0            | 2022-12-08 |
| 1202    | ESC_2             | 2022-12-08 | ESC_2            | 2022-12-08 | ESC_2            | 2022-12-08 | ESC_2            | 2022-12-08 |
| 0105    | LCPU              | 2023-05-11 | LCPU             | 2023-05-11 | LCPU             | 2023-05-11 | LCPU             | 2023-05-11 |
| 0500    | PD_MCU            | 2021-08-25 | PD_MCU           | 2021-08-25 | PD_MCU           | 2021-08-25 | PD_MCU           | 2021-08-25 |
| 1006    | SPEAKER_MCU       | 2022-11-23 | SPEAKER_MCU      | 2022-11-23 | SPEAKER_MCU      | 2022-11-23 | SPEAKER_MCU      | 2022-11-23 |
| 2607    | RTK982            | 2022-12-01 | RTK982           | 2022-12-01 | RTK982           | 2022-12-01 | RTK982           | 2022-12-01 |
| 0103    | ****              | ****       | ****             | ****       | Infrared         | 2022-11-24 | Infrared         | 2022-11-24 |
| 0106    | ****              | ****       | ****             | ****       | IR_USB_CONN      | 2022-07-13 | IR_USB_CONN      | 2022-07-13 |
+---------+-------------------+------------+------------------+------------+------------------+------------+------------------+------------+
```

Software version breakdown 
```
+---------+-------------------+------------+------------------+------------+------------------+------------+------------------+------------+
| Module  | wm265e            | Version    | wm265e           | Version    | wm265t           | Version    | wm265t           | Version    |
| ID      | (20.00.0005)      |            | (09.00.0505)     |            | (20.00.0005)     |            | (09.00.0505)     |            |
+---------+-------------------+------------+------------------+------------+------------------+------------+------------------+------------+
| 0802    | WM265E_E2         | 20.00.00.07 | WM265E_E2        | 11.05.02.05 | WM265T_E2        | 20.00.00.07 | WM265T_E2        | 11.05.02.05 |
| 1502    | WM265_E1E         | 20.00.00.04 | WM265_E1E        | 11.05.02.06 | WM265_E1E        | 20.00.00.04 | WM265_E1E        | 11.05.02.06 |
| 1100    | Battery           | 08.75.02.23 | Battery          | 08.75.02.23 | Battery          | 08.75.02.23 | Battery          | 08.75.02.23 |
| 1200    | ESC_0             | 01.90.01.27 | ESC_0            | 01.90.01.27 | ESC_0            | 01.90.01.27 | ESC_0            | 01.90.01.27 |
| 1202    | ESC_2             | 01.90.01.27 | ESC_2            | 01.90.01.27 | ESC_2            | 01.90.01.27 | ESC_2            | 01.90.01.27 |
| 0105    | LCPU              | 01.13.10.01 | LCPU             | 01.13.10.01 | LCPU             | 04.13.10.01 | LCPU             | 04.13.10.01 |
| 0500    | PD_MCU            | 05.02.22.46 | PD_MCU           | 05.02.22.46 | PD_MCU           | 05.02.22.46 | PD_MCU           | 05.02.22.46 |
| 1006    | SPEAKER_MCU       | 01.00.00.28 | SPEAKER_MCU      | 01.00.00.28 | SPEAKER_MCU      | 01.00.00.28 | SPEAKER_MCU      | 01.00.00.28 |
| 2607    | RTK982            | 00.00.79.80 | RTK982           | 00.00.79.80 | RTK982           | 00.00.79.80 | RTK982           | 00.00.79.80 |
| 0103    | ****              | ****       | ****             | ****       | Infrared         | 10.01.05.07 | Infrared         | 10.01.05.07 |
| 0106    | ****              | ****       | ****             | ****       | IR_USB_CONN      | 00.00.10.77 | IR_USB_CONN      | 00.00.10.77 |
+---------+-------------------+------------+------------------+------------+------------------+------------+------------------+------------+
```

R3E firmware should be compatable with M3E, and R3T firmware compatible with M3T accordingly. If you'd like to be a guinnea pig, please reach out via [Git Issue](https://github.com/MAVProxyUser/BizarreActorPoutsOn/issues/new/choose).

IF you are lucky an [OG](https://www.dji-rev.com) may help you out. You probably need to hit #spoon-feeding however. 

See the retroroms ["List of the Modules and What they Effect"](https://github.com/MAVProxyUser/BizarreActorPoutsOn/tree/main) for more detail. 

See also historic mirrors of the ["firm_cache"](https://github.com/chinger1313/firm_cache)

There is more than enough public info for you to accomplish your own flashing in the near term. Be careful. We are not responsible for damages, or butt hurt feelings! 

How did we determine the software was identical? 

First to analyze and compare this you need to know how to add a key to dji_imah_fwsig.py from dji-firmware-tools... (but you probably don't have the one you need)

["These specific keys were not integrated into list of keys found in the dji-firmware-tools script to decrypt and unpack the firmware, 
so we manually added them in the code as UFIE-2022-04 and TBIE-2022-04, respectively. With this addition, we were finally able to 
successfully decrypt the firmware using the manually added key UFIE-2022-04"](https://www.nozominetworks.com/blog/dji-mavic-3-drone-research-part-1-firmware-analysis)

[These are the firmware encryption keys that @DJIGlobal uses to hide their GPL violations on Mavic 3.](https://x.com/tmbinc/status/1509821668495179796)
"UFIE" = 56 CF 6D 75 7A 45 32 4C 6E 1D 97 85 41 5F 44 85
"TBIE" = FF B7 AC 5A 03 5B 0E F2 F4 1D CD B1 FC 66 FB 6B


['@tmbinc If I remove the signature length limit then I just get signature verification failed from dji_imah_fwsig.py and there are no hardcoded keys in that file that start with the first bytes of your UFIE key above. I added the keys above as UFIE-2022-08 and TBIE-2022-08 respectively. I still get the same error when I use them, e.g.](https://dji-rev.com/dji-rev/pl/g956dkffrt89z8r8cshgzbzhqe)

```
../../dji-firmware-tools/dji_imah_fwsig.py -vvv -u -i wm260_0802_v10.00.40.18_20220121.pro.fw.sig -k PRAK-2020-01 -k UFIE-2022-08 -k TBIE-2022-08
    "UFIE-2022-08":  bytes([ 
        0x56, 0xcf, 0x6d, 0x75, 0x7a, 0x45, 0x32, 0x4c, 0x6e, 0x1d, 0x97, 0x85, 0x41, 0x5f, 0x44, 0x85
    ]),
    "TBIE-2022-08":  bytes([ 
        0xff, 0xb7, 0xac, 0x5a, 0x03, 0x5b, 0x0e, 0xf2, 0xf4, 0x1d, 0xcd, 0xb1, 0xfc, 0x66, 0xfb, 0x6b
    ]),'
```

I just showed you how to add a key above, but the M3E key is private as I mentioned above. 

```
dev0:dji-firmware-tools SlackOG$ git diff
diff --git a/dji_imah_fwsig.py b/dji_imah_fwsig.py
index e9e5eb8..6967b5c 100755
--- a/dji_imah_fwsig.py
+++ b/dji_imah_fwsig.py
@@ -164,6 +164,16 @@ keys = {
     "SLEK":  bytes([ # Slack community Encryption Key; generated 2018-01-19 by Jan Dumon
         0x56, 0x79, 0x6C, 0x0E, 0xEE, 0x0F, 0x38, 0x05, 0x20, 0xE0, 0xBE, 0x70, 0xF2, 0x77, 0xD9, 0x0B
     ]),
+    # WM265e FW v11.07.01.16_20240625 - Anzu Raptor
+    "UFIE-RAPTOR":  bytes([ 
+        0xCENSORED, 0xSORRY
+    ]),
+    "UFIE-2022-08":  bytes([ 
+        0x56, 0xcf, 0x6d, 0x75, 0x7a, 0x45, 0x32, 0x4c, 0x6e, 0x1d, 0x97, 0x85, 0x41, 0x5f, 0x44, 0x85
+    ]),
+    "TBIE-2022-08":  bytes([ 
+        0xff, 0xb7, 0xac, 0x5a, 0x03, 0x5b, 0x0e, 0xf2, 0xf4, 0x1d, 0xcd, 0xb1, 0xfc, 0x66, 0xfb, 0x6b
+    ]),
```

If you need a quick refresher on using the unpacking tools, this should help
```
dev0:dji-firmware-tools SlackOG$ python3 dji_imah_fwsig.py -h
usage: dji_imah_fwsig.py [-h] [-i SIGFILE] [-m MDPREFIX] [-f] [-r] [-k KEY_SELECT] [-v] (-u | -s | --version)

DJI Firmware IMaH Un-signer and Decryptor tool

options:
  -h, --help            show this help message and exit
  -i SIGFILE, --sigfile SIGFILE
                        directory and file name of signed and encrypted IM*H firmware module (default is base name of mdprefix with extension sig appended, in working dir)
  -m MDPREFIX, --mdprefix MDPREFIX
                        directory and file name prefix for the single un-signed and unencrypted firmware module (default is base name of sigfile with extension stripped, in
                        working dir)
  -f, --force-continue  force continuing execution despite warning signs of issues
  -r, --random-scramble
                        while signing, use random scramble vector instead of from INI
  -k KEY_SELECT, --key-select KEY_SELECT
                        select a specific key to be used for given four character code, if multiple keys match this fourcc
  -v, --verbose         increases verbosity level; max level is set by -vvv
  -u, --unsign          un-sign and decrypt the firmware module
  -s, --sign            sign and encrypt the firmware module
  --version             display version information and exit
```

To unpack the firmware use the RAPTOR key that we added above (that you won't have)
```
dev0:dji-firmware-tools SlackOG$ python3 dji_imah_fwsig.py -i ~/Desktop/M3E_M3T_DJI-CDN_dump/wm265e_1502_v11.05.02.06_20231222.pro.fw.sig -k UFIE-RAPTOR -f -u 
dev0:dji-firmware-tools SlackOG$ python3 dji_imah_fwsig.py -i ~/Desktop/Aloft_DJI-CDN_dump/wm265e_1502_v20.00.00.04_20231212.pro.fw.sig -k UFIE-RAPTOR -f -u

dev0:dji-firmware-tools SlackOG$ tar tvf wm265e_1502_v11.05.02.06_20231222.pro.fw_1502.bin
-rw-rw-r--  0 0      0         122 Aug 24  2017 META-INF/com/android/metadata
-rw-rw-r--  0 0      0      619512 Aug 24  2017 META-INF/com/google/android/update-binary
-rw-rw-r--  0 0      0        4935 Aug 24  2017 META-INF/com/google/android/updater-script
-rw-rw-r--  0 0      0     2416640 Aug 24  2017 bootarea.img
-rw-rw-r--  0 0      0       18592 Aug 24  2017 file_contexts
-rw-rw-r--  0 0      0     7826272 Aug 24  2017 normal.img
-rw-rw-r--  0 0      0     4539008 Aug 24  2017 rtos.img
-rw-rw-r--  0 0      0   247595008 Aug 24  2017 system.new.dat
-rw-rw-r--  0 1002   1002        0 Aug 24  2017 system.patch.dat
-rw-rw-r--  0 0      0        1212 Aug 24  2017 system.transfer.list
-rw-rw-r--  0 0      0    98885632 Aug 24  2017 vendor.new.dat
-rw-rw-r--  0 1002   1002        0 Aug 24  2017 vendor.patch.dat
-rw-rw-r--  0 0      0         757 Aug 24  2017 vendor.transfer.list
-rw-rw-r--  0 0      0        1383 Aug 24  2017 META-INF/com/android/otacert
-rw-rw-r--  0 0      0        1891 Aug 24  2017 META-INF/MANIFEST.MF
-rw-rw-r--  0 0      0        1264 Aug 24  2017 META-INF/CERT.SF
-rw-rw-r--  0 0      0        1477 Aug 24  2017 META-INF/CERT.RSA

dev0:dji-firmware-tools SlackOG$ tar tvf wm265e_1502_v20.00.00.04_20231212.pro.fw_1502.bin
-rw-rw-r--  0 0      0         122 Aug 24  2017 META-INF/com/android/metadata
-rw-rw-r--  0 0      0      619512 Aug 24  2017 META-INF/com/google/android/update-binary
-rw-rw-r--  0 0      0        4935 Aug 24  2017 META-INF/com/google/android/updater-script
-rw-rw-r--  0 0      0     2416640 Aug 24  2017 bootarea.img
-rw-rw-r--  0 0      0       18592 Aug 24  2017 file_contexts
-rw-rw-r--  0 0      0     7821568 Aug 24  2017 normal.img
-rw-rw-r--  0 0      0     4539008 Aug 24  2017 rtos.img
-rw-rw-r--  0 0      0   247599104 Aug 24  2017 system.new.dat
-rw-rw-r--  0 1002   1002        0 Aug 24  2017 system.patch.dat
-rw-rw-r--  0 0      0        1212 Aug 24  2017 system.transfer.list
-rw-rw-r--  0 0      0    98873344 Aug 24  2017 vendor.new.dat
-rw-rw-r--  0 1002   1002        0 Aug 24  2017 vendor.patch.dat
-rw-rw-r--  0 0      0         757 Aug 24  2017 vendor.transfer.list
-rw-rw-r--  0 0      0        1383 Aug 24  2017 META-INF/com/android/otacert
-rw-rw-r--  0 0      0        1891 Aug 24  2017 META-INF/MANIFEST.MF
-rw-rw-r--  0 0      0        1264 Aug 24  2017 META-INF/CERT.SF
-rw-rw-r--  0 0      0        1477 Aug 24  2017 META-INF/CERT.RSA

```

These MD5's match directly 1:1 the other images would need to be extracted and compared. 
```
file_contexts
MD5: e61b3f3c3879b61761bb4d3ad98ef26d
system.patch.dat
MD5: d41d8cd98f00b204e9800998ecf8427e
vendor.patch.dat
MD5: d41d8cd98f00b204e9800998ecf8427e
META-INF/CERT.SF
MD5: 18c274bd8f4a4d1b254503c63ce07d39
META-INF/MANIFEST.MF
MD5: ba0f7cc692e3ee15646fdf42ca649aa7
META-INF/com/android/otacert
MD5: e5d999219205a1d30b4464c4bae21139
```

# Mitigation

Anzu Robotics / Aloft will need to obtain their own "keys" as described in the [DJI Drone Security White Paper 3.0](https://www.dji.com/trust-center/resource/white-paper), and burn them into their hardware accordingly. The following changes will need to be made: 

New root keys:
```
The root keys will be injected into the OTP to ensure confidentiality. When the keys are
transmitted, a unique secret key is used for encryption for every single DJI product, and the
corresponding decryption is performed in TEE. After the key is written, it can only be accessed by
the secure engine, and the software cannot access it, thus ensuring the confidentiality of the key.
```

New device certificates:
```
DJI products use X.509 format certificate, with each certificate bound to the drone’s SN. These
device certificates are mainly used for device authentication and access control in services
such as 4G enhanced transmission and device connection to the cloud.
```

Secure boot keys:
```
For every step in the boot process, the firmware is encrypted and signed by DJI to ensure its
confidentiality and integrity. The firmware can only run after it is verified and decrypted. The firmware
includes boot loaders, kernels, secure operating systems, flight control firmware, and others.
...
This secure boot chain ensures the integrity of the drone’s software system. 
```

Secure update keys:
```
DJI drones support remote system updates for new feature releases, bugs fixes, and security
vulnerability patches. The update package will be signed and encrypted by DJI before it is released.
The drone decrypts and verifies the signature of the update package, and begins the update
once verification is complete. The update system also supports a hardware-based anti-rollback
mechanism to prevent users from rolling back to vulnerable firmware versions
...
The secure update solution effectively prevents the installation and execution of malware on
the DJI drone, ensuring the reliability of the drone software.
```







