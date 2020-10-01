## Ethical Hacking: Understanding Ethical Hacking

This is a course that is offered for free (during the camp) by Pluralsight. I haven't reached the security part of the course yet, so I cannot say if I like it or not. The statistics are definitely interesting but the concept of using multiple virtual machines is quite indifferent to me, especially since I have no way to perform these operations on my own. I took this course as a free opportunity to learn what "ethical hacking" was (i.e. the [Github Bounty](https://bounty.github.com/)), etc., but so far I haven't had any hands-on experience. The notes are a great reference, but I am currently unable to apply them in real life. For those interested, you can take the course here:

> [Ethical Hacking: Understanding Ethical Hacking](https://www.pluralsight.com/courses/ethical-hacking-understanding)

Below are my notes for this course. Please note that these notes are like guidelines and *not* a replacement for the course. If you want to learn more about this topic, please use the link above.

### The Truth About Living in a Technology Based World

- Cyber attacks are expected to increase a *lot* between 2014 and 2017 (I forgot the exact number mentioned, but it will increase quite a bit).

### Overview of the CEH Certification Program

> If it wasn't "hard", everyone would do it...
> "Hard" is what makes "it" great &ndash; Tom Hanks

What's in it for me?

- Internationally recognized
- Industry standard (Meets DOD Directive 8570.1)
- Benefits your resume
- High demand certification

Maintain Your CEH with ECE Credits by:

- Attending conferences
- Writing research papers
- Community training / training sessions
- Reading related subject materials
- Exams (continuing your education)
- Attending webinars

One should never fake this information; always bring evidence just in case. Keep track of these events and submit them. The points are accumulative yearly from January 1st to December 31st. Make sure that these points are recorded before February 1st.

- You should record your ECE's with the ECE Delta/Aspen Portal.
- If you have questions regarding ECE credits, contact the EC-Counsel.

[Code of Ethics](http://www.eccouncil.org/support/code-of-ethics)

- Privacy
- Intellectual property
- Disclose information to the right people when needed
- Be honest about your Areas of Expertise
- Never unknowingly use software that are obtained unethically or illegally
- Illegal activities
- Authorization: Make sure your work is to their knowledge and consent
- If you come accross a flaw, notify the manufacturer. If the manufacturer does not respond, make sure to notify users of the problem.
- Management
- Knowledge Sharing (Study and share the things that you learn with other EC-Council members)
- Confidence with other 
- Extreme care with the software and other tools (Don't fix something without verification)
- Do not associate or engage in any activities considered malicious
- No compromise
- Make sure everything is within legal limits
- Do not promote blackhat activity (forums)
- Do not participate in underground communities

> "In order to understand the enemy, you've got to know what the enemy is doing and what they're up to."

It is important to review the [Candidate Agreement (CCA)](http://eccouncil.org/members/candidateagreement.pdf).

### How to Build a Lab to Hack Safely

> "Practice builds knowledge, knowledge builds confidence" &ndash; SuperDale

SuperDale Rules

- I promise NOT to "tryout" tools on my production network, competitors, or anyone who upsets me.
- I understand that neither the author nor PluralSight is responsible for my actions.
- "With great power comes great responsibility."

> Integrity: What you do when people aren't watching you.

Host Machine

- Virtualization: Hyper-V / VMware / VirtualBox
- Should have 32GB (16GB Minimum) RAM
- At least a 50GB of free space on hard drive (SSD Preferred)
- 1 Network Interface Card (NIC)

Setting Up

- 5 Virtual machines:
  - Windows 10
  - Windows 8.1
  - Windows 7
  - Windows Server 2008 R2
  - Windows Server 2012 R2
  - BackTrack / Kali (Pen Testing Product)
- Make sure that the virtual machines are on their own separate network and are NOT allowed to communicate with the host machine.
- [Kali website](https://www.kali.org/) (Use the Full version, 64 bit)
- Download an evaluation of Windows 7 with: tinyurl.com/ethicalW7P[1-7] where [1-7] represents the part number.

> The host machine should be running Windows Server 2012 with the GUI interface (don't use core). This will be used to install Hyper-V.

- Use a custom install and take the whole partition
- Avoid using a password such as`Pa$$w0rd`.
- Remember to change the computer name (requires reboot)
- Make sure to turn off SmartScreen and IE Enhanced Security Configuration (inside the Server Manager Dashboard)
- Open the control panel and navigate to Advanced system settings, then Advanced > Performance > Settings > Data Execution Prevention, and change the value so that it is only for "essential windows programs and services".
- Select the "Add Roles and Features Wizard", then select Hyper-V under Server Roles. Use all the defaults for the configuration. Upon reboot(s), open Hyper-V and select the Virtual Switch Manager. Select a private virtual switch so the machines can only talk to themselves.

### Installing and Configuring Your Windows Server VMs

Installing a VM with the Hyper-V Manager

- Select New > Virtual Machine
- Use Generation 1 for the Hyper-V Generation
- Use 4096 MB for each box; don't use dynamic memory
- Use the Virtual Switch Network that you created in the previous section
- Use the default storage settings
- Select to install an operating system from a bootable CD/DVD-ROM (.iso)

Repeat the steps in the previous section to install Windows Server 2012 R2 once more. Make sure to give the VM computer names general names such as "Server5".

### Installing and Configuring Your Desktop VMs

### Information Security Overview

### Security Threats and Attack Vectors

### Hacking Concepts

### Hacking Phases

### Attack Types

### Information Security Controls

### How to Prepare for the Certified Ethical Hacker Exam
