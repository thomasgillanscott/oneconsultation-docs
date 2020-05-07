# Using OneConsultation with iOS 13.4

We are aware of a potential issue with using OneConsultation with Safari, the default browser on Apple devices.

## Issue Description

The symptoms to look out for with this issue are the following:
	
 * Both users join the consultation.
 * Video works for both users.
 * The service user (using the Admin Portal)  cannot hear the public user (using the webpage).

The issue occurs when the public user does the following when joining the call:
	
* User goes to a OneConsultation service webpage- eg demo.oneconsultation.net and enables the website to access the microphone and speakers.
* Before clicking the "Begin Consultation" button, the user navigates to other Safari pages, then returns to the OneConsultation page. (This is not consistent, sometimes navigation in Safari does not cause this.)
* User clicks the "Begin Consultation" button and appears to join the conference in the usual manner.

The reason there is no audio from the patient is that at some point whilst navigating away from the OneConsultation web page, the connection to the microphone is lost but the user is not prompted to grant permission again.

## Resolution 

The fix is to close the existing web page and open a NEW page in Safari from the Apple device and then re-connect to the OneConsultation portal.  **It is important not to navigate away from this webpage once access to their microphone and webcam has been granted.**

This issue is with the iOS software so we continuing our investigations to determine the exact behaviour causing this but in the meantime, we will post instructions on the OneConsultation public portal to mitigate this problem.  These instructions will only be displayed for those users joining using an Apple device.
