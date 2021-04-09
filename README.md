# open-stethos
Open source digital smartphone stethoscope for remote patient monitoring.

I have an idea for an open source project, and I need help with it.
The project is an open source smartphone stethoscope.

This idea came to me, when my parents told me that they couldn't get to the doctor in 2021, due to the Covid pandemic that is hurting everyone for the last 16 months.
The doctor wasn't accepting patients, and they were caughting. The remote practice didn't involve listening to their lung with the stethoscope, because you cannot do that reliably over the phone.
I had the idea to make some hardware that would allow us to do this.

The project should have five parts:
1) PCB with microphone to connect to a smartphone (HW)
2) Smartphone application to record audio and guide patient to place the microphone the correct way (SW)
3) Physical integration (ME)
4) Acceptance in the medical community (GP)
5) Making it avaliable for people in need

I decided to select a smartphone as the platfor for this, because they have larger penetration than PCs.
It is also easyer to use for elderly people, no drivers to set, no windows audio settings.
The hardware should cheap and easily reproducable. And it should be plug and play for the users. No adpator cables, no Segger Jlink programmers.
It should be safe to use.
I dont want to turn this into a medical startup, I want this to be avaliable for everyone and hopefully save lives.

a) GP: Would you accept a MP3 file (for example) sent to you in email, describing which part of the lung the patient is currently monitoring, and would you use it for treatment?
b) General: should we re-use parts of a stethoscope (avaliableo on aliexpress for about 3 EUR)
c) ME: Should the device be integrated into the (so called) bell or does the sound make any difference at the end of the tubing
d) USB connection of a PCM29xx ADC/DAC is supported on Android. Does this work on iPhone? What cable is needed for this? 
e) Enclosure design, 3D printable. 
   Probably injection moulding would be an option if we want to make out many of these devices. 
   Using off the shelf enclosure? 
   Baloon as membrane?
f) What frequency range is nessesary to record? Should we filter outside this band?
g) TI's PCM2900C probably satisfies the requirements so it is selected for now
h) Mems microphone as default, with electret microphoe as substitute alternative
i) what happens if the phone sets the default audio output to the PCM2900 and there is no speaker. can we output instructions through phone speaker?
j) Smartphone development a can of worms


About me: I'm an EE who is familiar with PCB design, and have some experiance with medical devices.
License: MIT open source. Copy it, improve it, use it, help people.