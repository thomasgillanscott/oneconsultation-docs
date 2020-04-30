# Getting Started

*This is a technical document about how OneConsultation works, aimed at technical implementers and evaluators. For more general information about the problems that OneConsultation solves and how it can add value to your organisation, visit our [OneConsultation site](https://modalitysystems.com/software/oneconsultation).*

## What is OneConsultation?

OneConsultation is a fully managed, hosted service that enables professionals to conduct video consultations using Microsoft Teams or Skype for Business, with public users that are using only a web browser. 

## How is this different from using Skype for Business Meeting App?

Skype for Business Meeting App is designed for joining previously arranged and scheduled conferences organised in Microsoft Exchange. It assumes users have a level of experience with Skype for Business and requires a browser plug-in to work.

OneConsultation does not require a meeting to be created in Microsoft Exchange, does not assume the user has any prior experience with Skype for Business, and does not require any browser plug-ins.

## How is the video rendered within the browser?

WebRTC is used to present audio & video content to users in the browser. In order for this to work, users need to use a modern browser. A [matrix of supported clients is available](browsers.html).

## What is WebRTC?

WebRTC is the technology used to deliver plugin-less video consultations in a web browser. For more information, see [What is WebRTC?](webrtc.html)

## How are meetings created?
The public user is given a link to a portal page, that they can access via their internet browser, which asks them some pre-defined questions (these are configurable during the setup of OneConsultation). 

Once the public user has answered the questions, a new dynamic meeting is created, and the user is placed into the meeting. As the meeting is created on-demand by the user in this way, there is no requirement for them to provide a unique meeting ID, joining URL or PIN. 

As soon as the meeting has been created, it is displayed on the Admin Portal, enabling the Office 365 user to join the meeting using their Microsoft Teams or Skype for Business client. 

Here’s a real-world summary of the process using patients and clinicians as an example:  

- Patient is sent details of the online clinic with a single link to click on 
- Patient clicks on the link and answers some pre-defined questions 
- Patient joins a virtual waiting room (user is placed into dynamic meeting) 
- Clinician can see via the Admin Portal that the Patient is in the virtual waiting room 
- Clinician joins the Patient using their existing Microsoft Teams or Skype for Business client and the virtual consultation begins. 

## How does OneConsultation integrate with existing calendar management systems?
There is no requirement to integrate with existing calendar management systems. Calendar management and scheduling can continue to happen as normal, using existing systems. 

OneConsultation does not provide any calendaring or scheduling services. Consultations should be arranged as they are today, the only difference being that instead of attending a location in person, a user visits the portal URL to begin the consultation.

## What about Security?
All traffic is secured using SSL, including the initial request to setup the meeting, and the meeting join process. Customer questions are not stored at rest. For more information, see the dedicated [Security & Resiliance](security_and_resiliancy.html) section.

## Do you have APIs I can use?

There is an Admin API which exposes details of consultations that have been created and which can be joined. For more information and to sign-up, or discuss integration - [contact us](https://modalitysystems.com/software/oneconsultation)

-----

## Still have questions?
 
This documentation is still being compiled and you may have a question which is not answered here. Please contact us via the enquiry form on our [website](https://modalitysystems.com/software/oneconsultation) and we will respond. Your question will be added to this page in order to help others.
