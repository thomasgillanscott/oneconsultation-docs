# OneConsultation Configuration Options

## Pubic-facing Portal

All settings can be configured a a room level.

| Name          | Description   |
| ------------- |:-------------:|
| Internal Room Name                       | Name shown in the Admin Portal to identify the room |
| AD Group ID                              | If provided, only users in the specific AD Group will have access to the room. If blank, all users in tenant will have access.
| Questions                                | Questions shown to users prior to starting consultation. Answers from questions are shown in the Admin Portal to identify the consultation. Any number of questions can be used. All questions are free-text entry. |
| AuditInput                               | Wether the user-supplied answers are audited on new consultation. *Requires additional setup steps.*|
| AuditRestrictOnFail                      | If true, prevent consultation happening if audit record cannot be written.|
| BeginConsultationText                    | Text shown on the button to start consultation.|
| DisconnectURL                            | URL that the user is taken to when disconnecting from consultation. Can be used to direct user to survey page.|
| PortalIntroExplainingText                | Text shown on the initial page underneath the title text. |
| PortalLogoUrl                            | URL of logo to be shown on portal.|
| PortalTitle                              | Title text to be shown on portal.|
| Show Recording Button                    | Enable Admin Portal users to record consultations that take place in this room. *Requires additional setup steps.*|
| RecordingActive                          | Show or hide the Recording Message text. This is shown at the bottom of the page underneath the questions and is commonly used to provide a notice about recording. |
| RecordingMessage                         | Text of Recording Message text. Can include hyperlinks.|
| ShowUserIPAddress                        | If true, shows the IP of the user at the bottom of the page.|
| GatedEntry                               | Wether every consultation is checked and approved against an existing system, via API. *Requires additional setup steps.*|
| InConsultationRecordingLink              | For recorded consultations URL to recording policy.|
| InConsultationRecordingMessage           | For recorded consultations, message shown to users whilst recording is active.|

## Admin Portal

The following settings are configured at a tenant level and applied to all rooms in the tenant.

| Name          | Description   |
| ------------- |:-------------:|
| AdminPortalTitle              | The title of the Admin Portal, show at the top of the page once logged in.|
| Aging0Colour                  | Initial accent colour of consultations when they appear in the Admin Portal|
| Aging1Colour                  | Accent colour of consultation after Aging1Mins has expired.|
| Aging1Mins                    | Number of minutes.|
| Aging2Colour                  | Accent colour of consultation after Aging2Mins has expired.|
| Aging2Mins                    | Number of minutes.|
| Aging3Colour                  | Accent colour of consultation after Aging3Mins has expired.|
| Aging3Mins                    | Number of minutes.|
| NoParticipantColour           | Accent colour of consultation with no participants. |
| AllowSMSConsultation          | Allow Admin Portal users to send SMS messages with links to consultations. |
| JoinButtonText                | Text shown on the button used to join a consultation. |
| NoWaitingUsersText            | Message shown to signifiy no users waiting for a consultation. |
| NotificationText              | Message shown in desktop notification for new consultation. |
| ParticipantWording            | Text used to describe number of participants in meeting. |
| SMSConsultationMessage        | Default message used when sending SMS message.|
| SMSLinkFormat                 | Default link format used when sending SMS message.|
| ShowGroupSessions             | Show Group Sessions link.|
| ShowInternalJoinLink          | Show Internal Join link, enabling users to share a link to the Teams/Skype join button.|
| ShowMoveConsultationControl   | Enable users to move consultations between rooms. |
| ShowParticipantCount          | Show Participant count on consultation. |
| ShowPartnerJoinLink           | Show External Join link, enabling users to share a link to join consultation via WebRTC to external parties.|
| ShowRecordingsLink            | Show Link to Recordings.
| SystemCallsYou                | When joining a consultation, instead of supplying a SIP join link, system places incoming call to user. |
| multipleRoomsIntroText        | Wording used to signify multiple consultation rooms exist.|
| showRecordingDownloadLinks    | Allow users to download recordings.|
| useWebRTCJoinLink             | If false, users join consultation via SIP link in Teams/Skype client. If true, launches web interface to join consultation. |
| ShowConsultationDesktopShare  | If true, users can initiate Desktop Sharing in consultation. Requires modern browser. |
| UseTeamsWebLink               | If false, uses SIP link. If true, uses HTTP Teams join link.|

The following settings can be configured per-room

| Name          | Description   |
| ------------- |:-------------:|
ShowAdHocRecordingButton        | Show recording button on consultation. *Requires additional setup steps.*|
