# OpenSourceCar
Open Source hardware and software to replace OE hardware in virtually any vehicle except EVs.

While there is nothing in the Repo yet... I would like to explain this insane idea as best I can.

How everything has become proprietary and you DO NOT OWN the software that makes your car function, it's licensed to you. So technically you do not own the car. With that being said, this IS and most certaintly WILL be a very large undertaking.

I am not an engineer of any kind. I play in electronics and software more or less a hobby for me. With the complexity of modern vehicles, monitoring various sensors from the engine to cameras and audio. It would be nice if those of us like myself, could diagnose and repair a vehicle. Above all make changes for perfomance with out the need of a dealer or using aftermarket devices to alter a PCM. 

Take John Deere as a prime example. They have straight up prevented people from repairing their own equipment that cost from a few thousand to millions of dollars, they "license" the software to you and provide no way to interface with the system to diagnose or repair it. You must take it back to them or they come to you to repair your equipment. it is genuinely fucked up that they do this. The greed of this company is ridiculous. I can see the automotive industry forcing this too.

Mean while back in the automotive world some manufacturers have implemented software/hardware as a service model. To top it off they harvest data from and about you and "your" vehicle and use it for marketing and tracking. I don't remember which manufacturer specfically I think BMW... for a nominal annual fee you can have heated seats or performance increase just by updating a few variables in the vehicles control modules, that cost a few thousand a year. another example is GM you buy this 80~100k truck, but you want heated seats key less entry, and remote start. not only do you need an onstar subscription, you have to pay a subscription fee for the added features.

A lot of modern vehicles have a cellular connection so it can call "home" and report its issues. dealerships use this data not just to service the vehicle but also as a marketing tool. They will call you and tell you that your car has an issue and they will try to sell you the service, in addition to this they track the vehicle via GPS.

I started thinking about this insanity to nickel and dime everyone for any for every feature they want. So I began thinking about this project.

The idea is to create some generic hardware using FPGAs and MCUs where needed to replace the OE electronics. like the PCM(powertrain control module), BCM(body control module), TCM(transmission control module), IVI(in vehicle infotainment) and so forth. The best part of this is that every module would have extra unused I/Os turning the vehicle into a development platform.

Every module would be essentially identical in terms of the hardware. Even if it is overkill for the intended purpose. With additional I/Os for those who want to add, create, develop additional software or devices for a vehicle this would enable such creativity. and let's not forget the awesome vehicle customizations that can be done.

For the basis of the software I was thinking FreeRTOS, The communications protocol would be FlexCAN primarily for speed, for any and all GUI needs using Qt3D. After all, if this will be an open source project, lets use open source tools.

In terms of interfacing with the vehicles existing electrical system, there would need to be "dongles/adapters" made to match the vehicle. I realise there are a number of challenges here. 

With various implementations of cruise control on the software and hardware side, propriteary infortainment systems. I am sure some hardware may have propritery software embedded. Like a throttle body that utilizes a stepper or servo to actuate the butterfly. I am sure these issues can be overcome. I am equally confident, the community as a whole can generate better software, and able to reduce the number of exploits too.

As I said, I am not an engineer of any sorts. I am willing to buy some development boards and begin down this path and start learning, experimenting with developing a PCM / BCM for my own vehicle. after all you have to start some where, right?

It would be great to have some automotive EEs involved in the hardware design, Most certaintly software engineers that are better than myself. Who can create a "framework" for the project and make it "modular/plug-in" based architecture.

I know this is an outrageously ambitious idea. I also think its a worth while idea/project. I am confident there are aspects of this I have not thought about yet. That's why I am publicizing this thought, to hopefully start some brain storming.

The dealer specfic proprietary diagnostics and repair tasks needs to end. For them it is all about charging you more. Another example is on some vehicles today, you have to go to the dealer to reset the oil life after an oil change. That is absolutely absurd and unecessary.

If you're genuinely intersted in devoting some time to help get things going. create a pull request and lets have a conversation.
