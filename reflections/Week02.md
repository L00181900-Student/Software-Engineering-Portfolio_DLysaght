## Reflection #2 - 14/10/26, Task 2

### Model Selection: 

#### Brief A: Aegis Flight-Control Software Update - WATERFALL METHOD 

  - Requirement Stability: 
    - Requirements are described as "unusually" well understood/stable; very unlikely to change 
    - Failure mode and warning behavior are precisely specified by an engineering analysis, prior to development

  *JUSTIFICATION*: The Waterfall Method is best suited to projects that possess requirements that are unlikely to change radically and that can be provided upfront; whilst usually unrealistic, in this example, the requirements are stable and the expected behavior of the software update has been provided before development has commenced, bypassing the Waterfall Method's limitations.
         
  - Risk/Safety:
    - A defect in such software could endanger lives; cost of a discovered defect is extremely high

  *JUSTIFICATION:* In this example, formal verification and extensive, detailed documentation is imperative, as to avoid potential endangerment of the public and to suit the requirements of safety-critical systems. 
     
  - Timeline:
    - No competitive pressure to release quickly
    - Certification timelines dominate scheduling (duration: often 12 - 18 months)
    
  *JUSTIFICATION:* As necessary certification processes dictate the schedule and can span a long duration of time (12 - 18 months), a software process not hinged on rapid development and delivery is required. 

  - Customer Involvement:
    - High; client organization possesses a large, well-resourced quality assurance department, who expects extensive documentation at every stage

  *JUSTIFICATION:* The Waterfall Method's documentation processes ensure that the client organization shall have access to accurate records of every stage of development, as required. 

**CHOSEN RISK:** Project success is extremely important, as a fault in the system update could endanger lives. The Waterfall Method is at a disadvantage in this regard, as testing only happens at the very end of the project, and serious issues thusly surface extremely late. 

#########################

#### Brief B: Riverside Bakery Marketing Website - PROTOTYPING   

  - Requirement Stability:
    - Highly unstable; client is subject to frequently change her mind about various details related to the project
    - Client is, quote, "not exactly sure what it should look like"
   
  *JUSTIFICATION:* The Prototyping software process is most applicable and valuable in regard to clients/developers that do not have a clear outline of project requirements, algorithms, business rules, performance needs, etc. 
  
  - Risk/Safety:
    - No safety or regulatory dimension involved; no adherence to certification/formal validation required

  *JUSTIFICATION:* The Prototyping approach can lead to a draft of the system that contains unresolved/undetected errors being mistaken for the final project; in this instance, while an inconvenience and a potentially costly repair, no party is at risk should the system contain a defect. Thus, this disadvantage does not undermine Prototyping's applicability in this scenario. 

  - Timeline:
    - Client requires a live web-application within three weeks, before a local food festival; time pressure is present

  *JUSTIFICATION:* Outlined time constraints emphasize the need for rapid development and early user feedback. 
  
  - Customer Involvement:
    - Client is available to give feedback daily
    - Client is prone to changing their mind often

**CHOSEN RISK:** The Prototyping software process could be costly should the development team require training in how to correctly execute it. As well as this, this approach may take longer to produce a system, and therefore increase costs further. Client budget is stated to be small, so this approach could be financially infeasible. This may be circumvented, should the Prototyping approach be combined with another, more substantial software approach, eg. the Iterative approach.  

#########################

#### Brief C: CampusCircle Community App - ITERATIVE DEVELOPMENT 

  - Requirement Stability:
    - Founders have a rough outline of fundamental/"core" features
    - Founders expect requirements to change significantly after test users interact with early versions of the application
   
  *JUSTIFICATION:* Whilst the development team have an idea of the core features of the application, the requirements are expected to evolve with user feedback after students test the early/initial versions of the application; this lends well to Iterative Development's step-by-step refinement process. The development team also has a high emphasis on producing a *useable* application within a month, meaning it is of higher importance to produce a full set of features at a time, as opposed to feature-by-feature development, like that of *Incremental* Development. 
  
  - Risk/Safety:
    - No formal regulatory requirements, however the application must conform to basic data protection practices 

  *JUSTIFICATION:* As the requirement for formal verification and regulation is minimal and there are no major safety concerns should the software fail or contain a fault, developers can focus their attention primarily on the design and rapid development of the application, instead of documentation or formal approval.
  
  - Timeline:
    - Founders wish to release a useable application within a month and adapt after feedback gathering 
    - Founders aim to launch the application before the start of the next academic term
    - Time pressure is present; Founders are aware of a slower moving competitor that may release around the same time
    - Development team is co-located, but small 

  *JUSTIFICATION:* The development team wishes to establish themselves and the application amongst the student body before the launch of their competitors; as well as this due to the limited size of the development team there are less people to allocate work to, placing strain on development velocity. 
  
  - Customer Involvement:
    - High customer involvement; student feedback is required, as the Founders wish to adapt each iteration of the project to user feedback  

  *JUSTIFICATION:* The Iterative Development approach facilitates fast user feedback, allowing the development team to quickly absorb and adjust requirement changes for the next iteration if the application and produce a costumer-facing, student-tailored product. 

#########################

#### Hypothetical Project - Method Justification:

**PROJECT BRIEF: (LLM GENERATED)**

A small technology startup wants to develop a mobile application called FitTrack, designed to help university students manage their fitness, wellbeing and daily exercise routines.

The founders have identified some initial features, including:
- Creating personal fitness profiles.
- Tracking daily exercise and activity.
- Setting fitness goals.
- Viewing progress reports.
- Sharing achievements with friends.
  
However, they are unsure which features students would find most useful and expect requirements to evolve as students begin testing the application.

The startup hopes to release a working version within three months, as another fitness application aimed at university students is gaining popularity. They want to remain competitive and establish a user base before the next academic year.

The development team consists of six people, including two developers, a designer, a tester and two project managers. Team members work remotely across different locations.

Because the app collects personal information relating to users' activity and wellbeing, the founders recognise that privacy and data protection must be considered carefully. They also want sufficient documentation to ensure the application can be maintained and updated in the future.

**CHOSEN METHOD & JUSTIFICATION:** 
