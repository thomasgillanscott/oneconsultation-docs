# Getting Started

*This is a technical document about how OneConsultation works, aimed at technical implementers and evaluators. For more general information about the problems that OneConsultation solves and how it can add value to your organisation, visit our [OneConsultation site](https://oneconsultation.net).*

## What is OneConsultation?

OneConsultation is a fully managed, hosted service that enables professionals to conduct video consultations using Skype for Business, with users that are using only a web browser. 

## How is this different from using Skype for Business Meeting App?

Skype for Business Meeting App is designed for joining previously arranged and scheduled conferences organised in Microsoft Exchange. It assumes users have a level of experience with Skype for Business and requires a browser plug-in to work.

OneConsultation does not require a meeting to be created in Microsoft Exchange, does not assume the user has any prior experience with Skype for Business, and does not require any browser plug-ins.

## How is the video rendered within the browser?

WebRTC is used to present audio & video content to users in the browser. In order for this to work, users need to using a modern browser. A [matrix of supported clients is available](browsers.html).

## What is WebRTC?

WebRTC is the technology used to deliver plugin-less video consultations in a web browser. For more information, see [What is WebRTC?](webrtc.html)

## How are meetings created?
The process begins when a user visits the portal page and answers some pre-defined, configurable questions. At that point, a new dynamic meeting is created. The user is placed into the meeting. At the same time, the meeting is shown on the Admin Portal, enabling any authenticated user to join the meeting using the Skype for Business client.

Because the meeting is created on-demand by the user, there is no requirement for the user to provide a unique meeting ID, joining URL or PIN.

## How does OneConsultation integrate with existing calendar management systems?
There is no requirement to integrate with existing calendar management systems. Calendar management and scheduling can continue to happen as normal, using existing systems. 

OneConsultation does not provide any calendaring or scheduling services. Consultations should be arranged as they are today, the only difference being that instead of attending a location in person, a user visits the portal URL to begin the consultation.

## What about Security?
All traffic is secured using SSL, including the initial request to setup the meeting, and the meeting join process. Customer questions are not stored at rest. For more information, see the dedicated [Security & Resiliance](security_and_resiliancy.html) section.

## Do you have APIs I can use?

There is an Admin API which exposes details of consultations that have been created and which can be joined. For more information and to sign-up, visit the API Management Portal.

-----

## Still have questions?
 
This documentation is still being compiled and you may have a question which is not answered here. Please email your question to [labs@modalitysystems.com](mailto:labs@modalitysystems.com) and we will respond to it. Your question will be added to this page in order to help others.
