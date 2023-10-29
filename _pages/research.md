---
permalink: /research/
title: "Research"
---

My research improves the security of emerging computing systems and their interactions with physical spaces through system design, formal methods, and applied cryptography. Here is a summary of some of my research efforts.

## Ensuring the Safety and Security of IoT Environments [CCS'22, NDSS'23]

 <p align="center">
 <img src="/files/iotseer.png"
     style="display:block;
        width: 500px;
        height: auto;" />
 <br>
 <em>Physical interactions in IoT environments.</em>
 </p>


<!-- <p style="text-align: justify"> -->
IoT environments include safety-critical smart devices that are an attractive target for adversaries to put the user or environment at risk. To mitigate these risks, I developed two systems to protect IoT environments against IoT app physical interaction threats and spoofing attacks. 

First, I introduced IoTSeer, which combines app code analysis and dynamic analysis with new security policies to discover physical interaction vulnerabilities among IoT apps. In IoTSeer, I modeled each IoT app’s physical behavior through hybrid modeling and proposed a new composition algorithm to construct a model that describes the joint physical behavior of apps. Yet, the apps’ composite model displays both discrete and continuous behavior, rendering traditional verification methods (e.g., model checking) undecidable. To address this, I used optimization-guided falsification to validate if the apps’ composite model adheres to a set of safety and security policies represented with metric temporal logic. This work appeared at ACM CCS 2022.

While designing IoTSeer, I noticed the complex physical interactions between IoT sensors and actuators enable adversaries to evade prior IoT event verification systems. These systems extract physical fingerprints that define the relations between actuators and sensors to detect event spoofing and masking attacks in which an adversary creates inconsistencies between actuators’ physical and cyber states. By systematically analyzing the fingerprints of prior anomaly detection systems, I found that they ignore complex physical interactions between devices, enabling an adversary to evade these systems and launch attacks without getting detected. I then proposed two defenses, software patching and sensor placement, which prevent the evasion attacks through the interplay of physical modeling and formal analysis. This work appeared at NDSS 2023.
<!-- </p> -->


 <p align="center">
    <a href='https://www.youtube.com/watch?v=-KMfcjscsMo&t=16s&ab_channel=NDSSSymposium'>
      <img src="/files/evasion.png"
          style="display:block;
          width: 500px;
          height: auto;"
           alt="NDSS 2023 - Evasion Attacks and Defenses Presentation"
           style="display:block; margin-left: auto; margin-right: auto;" />
    </a>
    <br>
    <em>NDSS 2023 - Evasion Attacks and Defenses Presentation</em>
 </p>

## Enhancing the Privacy of Commodity IoT Devices [S&P'23]

<!-- <p style="text-align: justify"> -->
I found that the physical interactions of IoT devices can serve as proof-of-copresence and be used to establish cryptographic keys for secure communication between devices. Prior pairing techniques are unsuitable for IoT devices as they require trusted entities, user interaction, or shared homogeneous context. Thus, they are prone to a single point of failure, have limited usability, and need additional sensors. To address this, I proposed IoTCupid, a group pairing system for IoT devices with heterogeneous sensors. IoTCupid extracts temporal features from the timing difference between consecutive events and integrates a fuzzy clustering algorithm to derive a shared secret. It then derives a group key among devices through a partitioned group password-authenticated key exchange (GPAKE) scheme. IoTCupid’s partitioned GPAKE scheme involves encrypting the public keys with the shared secrets and an intermediate two-party Diffie-Hellman key exchange before deriving group keys. I showed that IoTCupid enables dynamic group generation while offering resiliency against man-in-the-middle, brute force, and denial of key exchange attacks. This work appeared at IEEE S&P 2023.
<!-- </p> -->

 <p align="center">
 <img src="/files/iotcupid.png"
     style="display:block;
        width: 500px;
        height: auto;" />
 <br>
 <em>Overview of IoTCupid.</em>
 </p>

<!-- <p style="text-align: justify"> -->
While developing IoTCupid, I noticed secure communication is not enough to ensure the privacy of IoT environments as emerging IoT devices create new attack surfaces. Thus, in my recent works currently under submission, I explored the privacy risks of emerging IoT devices through side-channel analysis, machine learning, and formal methods. First, I developed a remote side-channel attack against intermittent devices to infer privacy-sensitive information about the environment in which they are deployed. Second, I designed VadMax to find vulnerabilities in voice assistant (VA) platforms and showed that an adversary can eavesdrop on privacy-sensitive device states and prevent users from controlling devices.
<!-- </p> -->


## Discovering and Patching Semantic Bugs [NDSS'21, S&P'22, UsenixSec'23a, UsenixSec'23b]

<!-- <p style="text-align: justify"> -->
My collaborators and I investigated discovering and patching semantic (logic) bugs in robotic vehicles (RVs) and autonomous vehicles (AVs). We identified that prior works cannot prevent RVs from reaching undesired physical states due to logical flaws in their control software. To address this, we introduced a fuzzing approach to check whether RVs adhere to formally represented safety and security policies. We then developed an automated software repair framework to patch the RV control software, preventing policy violations. Lastly, we introduced a patch verification framework to ensure RV software patches do not introduce additional bugs. These works identified over 250 previously unknown bugs in open-source RV control software and assisted developers in patching them. In more recent work, we found AVs are vulnerable to adversarial driving maneuvers. We proposed a framework to find such maneuvers in an automated way with a robustness-guided approach
<!-- </p> -->


## Developing Efficient Digital Signatures [CCS'18, CNS'18, CNS'19, FC'19]

<!-- <p style="text-align: justify"> -->
I developed lightweight public key cryptographic schemes for emerging applications such as drones and medical devices. I proposed an efficient digital signature that exploits the multiplicative property of RSA trapdoor permutation. My collaborators and I proposed a new post-quantum digital signature using the additive homomorphism of generalized compact knapsack functions. I developed a signer-efficient digital signature by eliminating the ephemeral public key in Schnorr-like signatures with a distributed construction. Later, I found a vulnerability in a digital signature that allowed conducting universal forgery attacks and fixed it through a new framework. 
<!-- </p> -->

## Identifying Exploitative Monetization Schemes [UsenixSec'22, NDSS'24]

<!-- <p style="text-align: justify"> -->
In a recent collaboration, my collaborators and I  uncovered exploitative monetization of content on YouTube through a thematic analysis of international forums. Later, we shed light on an abusive operation in e-commerce platforms by analyzing the online forums, instructional material, and software used by abusive sellers and conducting semi-structured interviews with legal consultants and sellers experienced in e-commerce.
<!-- </p> -->

