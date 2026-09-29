## Reflection #1 - 22/09/26, Task 1

###What is Software:
- A set of instructions/commands that instruct a computer to do a specific task that serves it's users. Software is non-physical, and rather exists to make the hardware work as per user requirements and the device's specified purpose; it enables hardware to perform tasks efficiently. There are two types of software:
    - System Software: Software that operates directly on computer hardware and provides basic functionality to users, as well as to the other software, so that it may run correctly. 
    - Application Software: Software that performs special functions and/or provides functions that are much more than basic computer operations. Designed to perform a *specific* task for end-users, as opposed to managing the system as a whole.  
    (Definition sourced from GeeksforGeeks) 

- Software is a set of items forming a 'configuration': programs, documents, and data — not code 
alone
- Generic products: stand-alone systems marketed and sold to any customer who wants them 
(mobile apps, word processors, project management tools) — the developer decides what the 
software should do
- Customized products: software commissioned by a specific customer to meet their own needs 
(embedded control systems, air-traffic control) — the customer decides what the software should 
do and drives change requests
- Software diversity: there is no universal set of techniques that fits every kind of system — methods 
and tools depend on the application, the customer's requirements, and the development team's 
background (Definition from Lecture Notes) 

#########################

###What does Engineering add to Software?:
- Engineering Discipline: appropriate theories and methods to more aptly solve problems, while bearing in mind organizational and financial constraints
- Methods/tools to support *all* areas of software development (eg. Project management), not just the technical process

#########################

###Two Examples of Software:
- Discord: Chronically buggy with each update, so I would assume testing prior to release is a low priority 
- CurseForge: Extreme emphasis on convenience and ease of use when dealing with mass amounts of mods; usually requires limited button presses to function

#########################

## The Four Process Activities: RetailSync Case Study:

### Specification: Weak
#### Stage 1:
- IT director only held a singular one-hour meeting in order to determine the overall requirements for the entire system
- Minimal guidance, "Roughly what was needed" emphasizes the lack of depth in prior research for the system
- No written document; development team has no record of requirements to reference

#### Stage 2:
- Warehouse staff were not properly consulted about system requirements during the development period; developers decided their vague understanding of the overall requirements from the Kickoff Meeting was sufficient

#### Stage 3:
- The IT director mentioned a major requirement in passing that should have been gathered during the initial Kickoff Meeting (Secondary warehouse and alternative shelving/barcode system support); however, this requirement was not included in the original undocumented brief 

### Development: Missing 
#### Stage 2: 
- The development team is incredibly unorganized; with minimal coordination, no shared coding standard, no shared review standard and minimal communication, as the document states they worked largely independently of one and other
- Development team neglected to use separate branches for newly added features, instead relying on pushing code directly to a shared folder within the network (no version control). This subsequently lead to occasional overwrites of each other's work without noticing

#### Stage 3:
- Upon receiving news of the secondary warehouse and alternative barcode and shelving system requirements, the lead developer only vaguely estimates the additional time needed to complete said features ("probably add a few weeks" - how many weeks? Why only probably?) and did not revise the existing design model; instead, the new requirements are haphazardly added on top of the existing schema 

### Validation: Weak
#### Stage 4: 
- Bare minimum testing performed for a limited time only; two days prior to the original deadline leaves very little room for system-breaking bugs to be repaired. As well as this, the depth of testing is very shallow, as developers only fixed bugs they *personally* encountered; no assurance that all major errors have been accounted for and that all features work reliably, and as described
- "Basically working" does not elaborate on what did or did not work; too ambiguous
- No warehouse staff tested the system, despite that group being the primary user base
- No test cases were recorded during development

#### Stage 5:
- In the end the program did not satisfy user expectations nor needs, as the stock-transfer screens were inaccurate, the secondary warehouse's barcode format was rejected by the scanner integration, and two staff members simultaneously corrupted stock counts on accident due to their lack of familiarity and involvement with the new system 

### Evolution: Weak
#### Stage 5: 
- Development team, left without a buffer period to properly iron out system-breaking errors, now has to scramble to repair the issues encountered as quickly as possible; this ends up extending the project by a further three months

### Conclusion: Most Damage Overall
- I believe the chronic lack of organization and documentation is what made this project fail: 
    - The requirements gathered are too ambiguous and scarce; from the get-go the overall outline for the system was too unspecific 
    - No documentation whatsoever; no frame of reference for the project outline, requirements, changes made nor errors/bugs encountered during development. Nobody has a clear, universal idea as to what the system is, must do and the development process regarding it; this also means the company has no baseline for future projects that may be similar 
    - The team itself seems loosely managed, with a distinct lack of communication and collaboration from all 3 parties. As well as this, due to the lack of a proper version control, multiple overwrites of code occurred, which is liable to corrupt key files the system relies on to function. Time management was also not employed during this project, as the development team only left itself 2 days to fully test the system for bugs 

#########################

## Researching a Software Failure: The Morris Worm (November 2nd, 1988) 

- The Morris Worm was a self-replicating computer program designed by at the time 23-year-old Robert Tappan Morris, a talented Cornell University graduate with a particular aptitude for Unix OS. He was also a notable prankster, and upon acceptance into Cornell University in August of 1988, he began development of a computer program that could secretly spread across the internet, unbeknownst to the user. He launched the program on a hacked MIT computer, which he accessed through his Cornell terminal in Ithaca, New York, presumably in an attempt to cover his tracks. 
- A computer *worm*, unlike a computer *virus*, does not require a software host, and instead is capable of existing and multiplying independently. Thusly, the Morris Worm could infect computers at a stark rate; within the first 24 hours of launch, an estimated 6,000 of the 60,000 computers that were connect to the Internet had been attacked. At this pace, the Morris Worm attack was able to successfully infiltrate a number of university and military functions, consuming all available processor and memory resources by repeatedly re-infecting the systems, slowing them to a crawl or, in some cases, crashing them completely.
- The worm initially only targeted systems of a specific Unix OS model; however, it spread much more broadly due to it's array of attack methods. For example, one of the ways the Morris Worm could spread was by exploiting a backdoor in the Internet's electronic mail system and a bug in the Unix "finger" user-information program that identified users on the system/network.
- The Morris Worm was not intended by Robert to be harmful in any manner; the program was not designed to harm the network, nor destroy local files or gain unlawful access to confidential information. On the contrary; the Morris Worm incident was the result of a coding oversight. The worm was programmed to enter a system and then check if the infection was already present, with a small catch; Morris asked the program to then replicate itself 14% of the time, regardless of whether the computer was already actually infected or not. The program, upon finding an already infected system, did not simply move onto the next- this resulted in a plethora of systems being infected and re-infected multiple times, each time bogging the hardware down further. The worm ran rogue for roughly 72 hours before researchers at Purdue and Berkley University were able to eliminate it.
- Robert Morris was the first person to be convicted under the relatively new *Computer Fraud and Abuse Act* of 1986, which outlawed unauthorized access to protected or otherwise private computers. However, most recognized Morris' good intentions and earnest remorse, and he was charged only with a single felony count, three years of probation, 400 hours of community service and a $10,000 fine in place of jail time. 
- The Morris Worm incident hearkens back to point 4 of the *'Characteristics & Importance of Software Engineering'* slides in that- while it may not have existed to serve any specific user- one must always ensure through proper testing that the program developed does not contain any fatal errors or major security issues. Code should be checked and tested thoroughly, especially when developing a program that accesses networks at large. 

### Sources: 
- [The Morris Worm (FBI, 02/11/2018)](https://www.fbi.gov/news/stories/morris-worm-30-years-since-first-major-attack-on-internet-110218)
- [Throwback Attack: The Morris Worm launches the first major attack on the internet (Control Engineering, 09/09/2021)](https://www.controleng.com/throwback-attack-the-morris-worm-launches-the-first-major-attack-on-the-internet/)

#########################
