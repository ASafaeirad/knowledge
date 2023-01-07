#software #requirement

Many different approaches to collaborative requirements gathering have been proposed. Each makes use of a slightly different scenario, but all apply some variation on the following basic guidelines:

- Meetings (either real or virtual) are conducted and attended by both software engineers and other stakeholders.
- Rules for preparation and participation are established.
- An agenda is suggested that is formal enough to cover all important points but informal enough to encourage the free flow of ideas.
- A “facilitator” (can be a customer, a developer, or an outsider) controls the meeting.
- A “definition mechanism” (can be worksheets, flip charts, or wall stickers or an electronic bulletin board, chat room, or virtual forum) is used.

The goal is to identify the problem, propose elements of the solution, negotiate different approaches, and specify a preliminary set of solution requirements.

A one- or two-page “product request” is generated during inception (Section 7.2). A meeting place, time, and date are selected; a facilitator is chosen; and attendees from the software team and other stakeholder organizations are invited to participate. If a system or product will serve many users, be absolutely certain that requirements are elicited from a representative cross section of users. If only one user defines all requirements, acceptance risk is high (meaning there may be several other stakeholders who will not accept the product). The product request is distributed to all attendees before the meeting date.

As an example, consider an excerpt from a product request written by a marketing person involved in the SafeHome project. This person writes the following narrative
about the home security function that is to be part of SafeHome:

> Our research indicates that the market for home management systems is growing at a rate of 40 percent per year. The first SafeHome function we bring to market should be the home security function. Most people are familiar with “alarm systems,” so this would be an easy sell. We might also consider using voice control of the system using some technology like Alexa. The home security function would protect against and/or recognize a variety of undesirable “situations” such as illegal entry, fire, flooding, carbon monoxide levels, and others. It’ll use our wireless sensors to detect each situation, can be programmed by the homeowner, and will automatically contact a monitoring agency and the owner’s cell phone when a situation is detected.

In reality, others would contribute to this narrative during the requirements gathering meeting and considerably more information would be available. But even with additional information, ambiguity is present, omissions are likely to exist, and errors might occur. For now, the preceding “functional description” will suffice.

While reviewing the product request in the days before the meeting, each attendee is asked to make a list of objects that are part of the environment that surrounds the system, other objects that are to be produced by the system, and objects that are used by the system to perform its functions. In addition, each attendee is asked to make another list of services (processes or functions) that manipulate or interact with the objects. Finally, lists of constraints (e.g., cost, size, business rules) and performance criteria (e.g., speed, accuracy, security) are also developed. The attendees are informed that the lists are not expected to be exhaustive but are expected to reflect each person’s perception of the system.

Objects described for SafeHome might include the control panel, smoke detectors, window and door sensors, motion detectors, an alarm, an event (a sensor has been
activated), a display, a tablet, telephone numbers, a telephone call, and so on. The list of services might include configuring the system, setting the alarm, monitoring the sensors, dialing the phone using a wireless router, programming the control panel, and reading the display (note that services act on objects). In a similar fashion, each attendee will develop lists of constraints (e.g., the system must recognize when sensors are not operating, must be user friendly, must interface directly to a standard phone line) and performance criteria (e.g., a sensor event should be recognized within
1 second, and an event priority scheme should be implemented).

The lists of objects can be pinned to the walls of the room using large sheets of paper, stuck to the walls using adhesive-backed sheets, or written on a wall board.
Alternatively, the lists may have been posted on a group forum or at an internal website or posed in a social networking environment for review prior to the meeting.
Ideally, each listed entry should be capable of being manipulated separately so that lists can be combined, entries can be deleted, and additions can be made. At this stage,
critique and debate are strictly prohibited. Avoid the impulse to shoot down a customer’s idea as “too costly” or “impractical.” The idea here is to negotiate a list that
is acceptable to all. To do this, you must keep an open mind.

After individual lists are presented in one topic area, the group creates a combined list by eliminating redundant entries, adding any new ideas that come up during the
discussion, but not deleting anything. After you create combined lists for all topic areas, discussion—coordinated by the facilitator—ensues. The combined list is shortened, lengthened, or reworded to properly reflect the product or system to be developed. The objective is to develop a consensus list of objects, services, constraints, and performance for the system to be built.

In many cases, an object or service described on a list will require further explanation. To accomplish this, stakeholders develop mini-specifications for entries on the lists or by creating a use case (Section 7.4) that involves the object or service. For example, the mini-spec for the SafeHome object Control Panel might be:

> The control panel is a wall-mounted unit that is approximately 230 × 130 mm in size. The control panel has wireless connectivity to sensors and a tablet. User interaction occurs through a keypad containing 12 keys. A 75 × 75 mm OLED color display provides user feedback. Software provides interactive prompts, echo, and similar functions. 

The mini-specs are presented to all stakeholders for discussion. Additions, deletions, and further elaboration are made. In some cases, the development of mini-specs will uncover new objects, services, constraints, or performance requirements that will be added to the original lists. During all discussions, the team may raise an issue that cannot be resolved during the meeting. An issues list is maintained so that these ideas will be acted on later.


📕 Case Study Example
Conducting a Requirements Gathering Meeting

The scene: A meeting room. The first requirements gathering meeting is in progress.

**The players:** Jamie Lazar, software team member; Vinod Raman, software team member; Ed Robbins, software team member; Doug Miller, software engineering manager; three members of marketing; a product engineering representative; and a facilitator.

**The conversation:**

**Facilitator (pointing at whiteboard):** So that’s the current list of objects and services for the home security function.
**Marketing person:** That about covers it from our point of view.
**Vinod:** Didn’t someone mention that they wanted all SafeHome functionality to be accessible via the Internet? That would include the home security function, no?
**Marketing person:** Yes, that’s right . . . we’ll have to add that functionality and the appropriate objects.

**Facilitator:** Does that also add some constraints?
**Jamie:** It does, both technical and legal.
**Production rep:** Meaning?
**Jamie:** We better make sure an outsider can’t hack into the system, disarm it, and rob the place or worse. Heavy liability on our part.
**Doug:** Very true.
**Marketing:** But we still need that . . . just be sure to stop an outsider from getting in.
**Ed:** That’s easier said than done and . . .
**Facilitator (interrupting):** I don’t want to debate this issue now. Let’s note it as an action item and proceed.
(Doug, serving as the recorder for the meeting, makes an appropriate note.)
**Facilitator:** I have a feeling there’s still more to consider here.
(The group spends the next 20 minutes refining and expanding the details of the home security function.)