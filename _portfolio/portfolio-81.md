---
title: "Liveness Detection"
excerpt: "Liveness Detection"
collection: portfolio
---

![Descriptor](/images/liveness.jpg){:height="450px" width="300px"}

## Description

Online Banks are claiming for this.  They want to be able to identify that an actual person is behind a mobile phone and is trying to register into a mobile app, to get a banking account, to issue a mortgage and so on.  It is not exactly recognizing who the person is against some previous record based on the picture of the face.  It is understaing that the picture is not fake, that the person is not wearing a mask, that it is there live and breathing.  It is a anti-spoofing approach. This project also connects with international developments like UBI or Worldcoin, because they need the liveness detection to implement their protocols to identify uniquely each person. 

* *Project*: The idea of this project is first to implement a desktop application based on OpenCV/YOLO stack that uses the camera from the computer to perform liveness detection.  It is also interesting to use the mobile camera to do the same.  The final scope is to perform all that using only javascript in a web app and do that offline withtout the intervention of any server side component.

* *Scope*:  the first steps towards the MVP is to have an application running either in a desktop app or in a mobile phone.

## Objective 

This problem has three sides.  The first one is this, the liveness detection.  This is an anti-spoofing tool that uses all the available transducers to get information that can give an idea that there is a real person on the other side.  This is similar to a captcha.  And this is an arms race.

The second axis is the authentication itself.  This is proving that THAT particular person over there, is the one who actually has some piece of information that can be verified against an internal database where some complementary information is encoded (this is for instance a password verification).  This is a mere authentication problem (with 1, 2, o any number of factors).

The final axis, is the verification that that ALIVE person over there, who has something that was originally registered in our systems, is actually a LEGAL person with a legal name and national id registered in a centralized manner in official government records.  This last part also connects this problem with UBI or worldcoin, which is a decentralized approach based on blockchain to do the same.

## Details

The initial onboarding registration processes require a first step where the physical person's identity is verified against government records. The goal is to confirm that the person registering is who they claim to be. This involves validating the data against government records, typically through consistency checks and biometric validation.

Additionally, the advancement of cell phones and the ubiquity of cameras in tablets and notebooks have driven the widespread use of facial recognition-based mechanisms. After fingerprint identification, facial recognition is currently the most used method.

In this context, biometric spoofing appears: a technique that attempts to deceive biometric systems into recognizing an illegitimate identity as genuine by presenting synthetic false alternatives based on the original directly to the biometric sensor.

This is an unresolved area, often categorized in security as side-channel attacks. These scenarios are the most challenging to address. For this reason, they are intensely researched both academically and from the technological perspective of developing commercial solutions.

In biometric identification or authentication mechanisms:

* Biometric information is public and cannot be modified.
* The types of attacks that can be implemented require a low entry bar, turning many potential users into possible attackers.
* Being side-channel attacks, digital protection systems are complementary but inherently insufficient.

Therefore, solutions often involve implementing artificial intelligence or machine learning to infer characteristics of the acquisition process that allow for the identification of synthetic forgery.

The types of attacks that can be carried out include direct attacks or side-channel attacks on the capture device or directly on the biometric data (biometric sample).

Attacks on the biometric data involve intercepting the data once it has been captured. This includes altering the recognition pipeline, tampering with the transmission of the information, altering its storage, etc.

Attacks on the capture device include tampering with the specific sensor (e.g., CCD cameras) or injecting non-fresh biometric material, implementing replay attacks.

However, both devices and storage and transmission media are often protected by cryptographic mechanisms that an attacker must overcome to gain access. Thus, as “the security chain is only as strong as its weakest link,” direct biometric spoofing attacks are currently the simplest direct alternative to apply.

Direct Biometric Face Spoofing attacks are typically classified into:

* Photo Attack: presenting a 2D image to the CCD sensor, printed on a sheet of paper, or displayed on a tablet, attempting to deceive the system with the photo of the falsified subject.
* Video Attack: presenting a 2D image that allows for a dynamic validation scenario, where, for example, blinking, lip movements, and head movements can be included. This includes challenge-response scenarios where a simple application allows the attacker to implement the different mechanisms requested by the application.
* Masks: recently popular in the Hong Kong protests, ranging from printed sheets with fake faces placed over a real face profile (addressing depth checks) to 3D models with the texture of the face to be falsified printed on them.

Multifactor Biometrics: similar to multifactor authentication, biometric processes that explore different factors simultaneously, such as a fingerprint alongside facial recognition, assume that the attacker needs to synthesize that biometric information, which is usually in different channels.

Specialized Sensors: "liveness detection" or "vitality detection" aims to detect intrinsic or involuntary information by measuring some biological process. For example, modifying the sensor to add infrared sensitivity to detect variations in red intensity corresponding to the pulse.

Digital: or based on the feature space. This is the most explored approach, addressing the problem as a machine learning classification problem. It can be static, dynamic, or implementing a challenge-response mechanism, generating interactivity with the subject (with a usability penalty).

Scoring: traditional fraud detection mechanisms, very popular in credit card transaction scenarios or actuarial settings. Viewing each identification process as a transaction that is scored and added to a data corpus, then addressed by global data analysis (i.e., analytics or data science).

There is an old adage in computer security that it is a bad idea to develop your own computer security system. The incentive for this approach is when considering a long-term process of evolution and continuous maintenance, or being aware of the inherent vulnerabilities such a system can have, accepting them as a valid and tolerable risk for the system in question.

Additionally, due to the nature of the problem, we see an innovative component in this development aiming to provide a technical solution that does not exist today or lacks the necessary maturity. This inevitably requires an iterative process and a long-term approach to the solution.

We recommend the possibility of implementing a hybrid solution (offline/online) that leverages server-side processing capabilities. The ability to deploy hardware resources accessible to an entity like a bank allows for raising the security bar.

Thus, the offline implementation provides a feasible solution that primarily operates as a backup system. From a programming perspective, the system can study and implement a trade-off between latency and processing time, choosing the best option to offer the user the best experience in performance, speed, data usage, and usability.

On the other hand, when implementing a security mechanism, it is necessary to understand what is being avoided. In this case, it is necessary to outline an initial Threat Model to understand the types of attacks, categorized by attack level.

To do this, it is necessary to understand the current state of productive systems: what types of attacks have been detected so far, under what contexts, and the system's current success in detecting them.

We consider this point crucial beyond the results obtained with a specific set of datasets, allowing for a more general approach to security, which is usually recommended (as security is a global property implemented with local checks).



# Some links
* [Servicio RENAPER](https://www.argentina.gob.ar/sid-sistema-de-identidad-digital)
* [Face++](https://www.faceplusplus.com/face-based-identification/)
* [Cognitive with Azure](https://docs.microsoft.com/en-us/azure/cognitive-services/face/face-api-how-to-topics/how-to-use-headpose)

# Papers 
* Abbas Ur Rehman, "LiveNet: Improving features generalization for face liveness detection using convolution neural networks", 2018
* Javier Galbally, "Biometric Antispoofing Methods: A Survey in Face Recognition", 2014
* Galbally, J., Marcel, S. and Fierrez, J., 2014. Biometric antispoofing methods: A survey in face recognition. IEEE Access, 2, pp.1530-1552.
* Mazzucato, M., 2019.Catch-up and Mission-oriented Innovation.How Nations Learn: Technological Learning,Industrial Policy,and Catch-Up, p.63
* https://fg2020.org/ 
* Marcel, S., Nixon, M.S. and Li, S.Z., 2014. Handbook of biometric anti-spoofing (Vol. 1). New York: Springer. 
* Chakraborty, S. and Das, D., 2014. An overview of face liveness detection. arXiv preprint arXiv:1405.2227.
* Li, K.C., Chen, X. and Susilo, W. eds., 2019. Advances in Cyber Security: Principles, Techniques, and Applications. Springer.
* https://fortune.com/2019/10/04/hong-kong-protests-mask-ban-surveillance-anonymity-facial-recognition/
* Ferguson, N. and Schneier, B., 2003. Practical cryptography (Vol. 141). New York: Wiley.
* Yallamandaiah, S. and Nalluri, P., 2019, September. Comprehensive analysis of face recognition techniques: A survey. In Computer-Aided Developments: Electronics and Communication: Proceeding of the First Annual Conference on Computer-Aided Developments in Electronics and Communication (CADEC-2019), Vellore Institute of Technology, Amaravati, India, 2-3 March 2019 (p. 149). CRC Press.





