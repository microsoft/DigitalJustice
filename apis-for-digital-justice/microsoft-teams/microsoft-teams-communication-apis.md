## Communication in Virtual Hearings

Communications API is perfect to build service applications (bots) that act like participants in a virtual hearing's call, and that create and retrieve meetings on behalf of users. This API provides calling functionality as well as the ability to create and retrieve online hearings. You can use service applications (bots) with this API, where the bot can act as a participant in your Microsoft Teams hearings, for example.

* [Call Resource Type](https://docs.microsoft.com/en-us/graph/api/resources/call?view=graph-rest-1.0): The call resource is created when there is an incoming call for the application or the application creates a new outgoing call via a `POST` on `app/calls`.
  * [Get](https://docs.microsoft.com/en-us/graph/api/call-get?view=graph-rest-1.0)
  
  * [Delete](https://docs.microsoft.com/en-us/graph/api/call-delete?view=graph-rest-1.0)
  
  * [KeepAlive](https://docs.microsoft.com/en-us/graph/api/call-keepalive?view=graph-rest-1.0)
  
  * [Answer](https://docs.microsoft.com/en-us/graph/api/call-answer?view=graph-rest-1.0)
  
  * [Reject](https://docs.microsoft.com/en-us/graph/api/call-reject?view=graph-rest-1.0)
  
  * [Redirect](https://docs.microsoft.com/en-us/graph/api/call-redirect?view=graph-rest-1.0)

* [Participant Resource Type](https://docs.microsoft.com/en-us/graph/api/resources/participant?view=graph-rest-1.0): Represents a participant in a virtual hearing's call.
  * [List](https://docs.microsoft.com/en-us/graph/api/participant-get?view=graph-rest-1.0)

  * [Get](https://docs.microsoft.com/en-us/graph/api/participant-get?view=graph-rest-1.0)
  
  * [Delete](https://docs.microsoft.com/en-us/graph/api/participant-delete?view=graph-rest-1.0)
  
  * [Mute participant](https://docs.microsoft.com/en-us/graph/api/participant-invite?view=graph-rest-1.0)
  
  * [Invite participant](https://docs.microsoft.com/en-us/graph/api/participant-invite?view=graph-rest-1.0)

* [Screen Share](https://docs.microsoft.com/en-us/graph/api/call-changescreensharingrole?view=graph-rest-1.0&tabs=http): Allow applications to share screen content with the participants of a virtual hearing group call.

* [Mute Application](https://docs.microsoft.com/en-us/graph/api/call-mute?view=graph-rest-1.0&tabs=http): Allows the application to mute itself. This is a server mute, meaning that the server will drop all audio packets for this participant, even if the participant continues to stream audio.

* [Unmute Application](https://docs.microsoft.com/en-us/graph/api/call-unmute?view=graph-rest-1.0&tabs=http): Allow the application to unmute itself. This is a server unmute, meaning that the server will start sending audio packets for this virtual hearing's call participant to other participants again.

* [Update Recording Status](https://docs.microsoft.com/en-us/graph/api/call-updaterecordingstatus?view=graph-rest-1.0&tabs=http): Update the application's recording status associated with a virtual hearing call. This requires the use of the [Teams policy-based recording](https://docs.microsoft.com/en-us/MicrosoftTeams/teams-recording-policy) solution.

* [Teleconference Device Quality Logging](https://docs.microsoft.com/en-us/graph/api/call-logteleconferencedevicequality?view=graph-rest-1.0&tabs=http): Logs video teleconferencing device quality data.

## Virtual Hearing's Call Recording

Call records provide usage and diagnostic information about virtual hearing's calls and online meetings that occur within your organization when using Microsoft Teams. You can use the call records APIs to subscribe to call records and look up call records by IDs.

* [Call Record Resource Type](https://docs.microsoft.com/en-us/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0): Represents a single peer-to-peer call or a virtual hearing group call between multiple participants.

  * [Get callRecord](https://docs.microsoft.com/en-us/graph/api/callrecords-callrecord-get?view=graph-rest-1.0)

* [Session Record Type](https://docs.microsoft.com/en-us/graph/api/resources/callrecords-session?view=graph-rest-1.0)

  * [List](https://docs.microsoft.com/en-us/graph/api/resources/callrecords-session?view=graph-rest-1.0)

* [Segment Record Type](https://docs.microsoft.com/en-us/graph/api/resources/callrecords-segment?view=graph-rest-1.0)

## Virtual Hearing's Online Meetings

* [Online Meeting Resource Type](https://docs.microsoft.com/en-us/graph/api/resources/onlinemeeting?view=graph-rest-1.0): Contains information about a virtual hearing call, including the URL used to join a meeting, the attendees list, and the description.
  
  * [Create onlineMeeting](https://docs.microsoft.com/en-us/graph/api/application-post-onlinemeetings?view=graph-rest-1.0)

  * [Get onlineMeeting](https://docs.microsoft.com/en-us/graph/api/onlinemeeting-get?view=graph-rest-1.0)

  * [Delete onlineMeeting](https://docs.microsoft.com/en-us/graph/api/onlinemeeting-delete?view=graph-rest-1.0)

  * [Create or Get onlineMeeting](https://docs.microsoft.com/en-us/graph/api/onlinemeeting-createorget?view=graph-rest-1.0)

## Presence

* [Presence Resource Type](https://docs.microsoft.com/en-us/graph/api/resources/presence?view=graph-rest-1.0): Contains information about a user's presence, including their availability and user activity.

  * [Get presence](https://docs.microsoft.com/en-us/graph/api/presence-get?view=graph-rest-1.0)

  * [Get presence of multiple users](https://docs.microsoft.com/en-us/graph/api/cloudcommunications-getpresencesbyuserid?view=graph-rest-1.0)