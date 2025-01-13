# OpenSourceCar
Open Source hardware and software to replace OE hardware in virtually any vehicle

While there is noting in the Repo yet... I would like to explain this insane idea as best as i can.

With how everything has become proprietary and you DO NOT OWN the software that makes your car function, its licensed to you. With that being said, this IS/WILL be a very large undertaking.

I am not an engineer of any kind, I play in electronics and software more or less a hobby for me. With the complexity of modern vehicles monitoring various sensors from the engine to cameras and audio it would be nice if those of us like myself could diagnose and repair a vehicle and above all make changes for perfomance with out the need of a dealer. take John Deere as a prime example. They have straight up put prevented people from repairing their own tractors that cost from a few thousand to millions of dollars, they "license" the software to you so to repair it you must take it back to them or they come to you to repiar your tractor it is genuinely fucked up that they do this. 

Mean while back in the automotive world some manufacturers have implemented software/hardware as a service model. To top it off they harvest data from and about you and "your" vehicle and use it for marketing and tracking. I don't remember which manufacturer specfically I think BMW... for a nominal annual fee you can have heated seats or performance increase just by updating a few variables in the vehicles control modules.

I started thinking about this insanity to nickel and dime everyone for any or every feature they want. I began thinking about this project.

The idea is to create some generic hardware using FPGAs and MCUs where needed to replace the OE electronics. like the PCM, BCM, TCM and so fourth.

Every module would have be essentially identical to every other one in terms of the hardware even if it is overkill with additional I/Os for those who want add, create develop additional software or devices for a vehicle. 

For the basis of the software I was thinking FreeRTOS and for any and all GUI needs using Qt. After all if this will be an open source project lets use open source tools.

In terms of interfacing with the vehicles existing electrical system, there would need to be "dongles/adapters" made to match the vehicle. I realise there are a number of challenges here with various implementations of cruise control and I am sure sure hardware may have propritery software embedded like a throttle body that utilizes a stepper or servo to actuate the butterfly. I am sure these issues can be overcome. I am equally confident that the community as a whole can generate better software with fewer exploits too.

As I said, I am no engineer of any sorts. but I am willing to buy some development boards and begin down this path and start learning and experimenting with developing a PCM and a BCM for my own vehicle. after all you have to start some where, right?

It would be great to have some automotive EEs involed in the hardware design and most certaintly software engineers that are better than myself.
Who can create a "framework" for the project and make it "plug-in"/modular based.

I know this is an outrageous idea but I also think its a worth while idea/project. I am more than sure there are aspects of this I have not thought about yet and thats why I am publicizing this thought. 

If your genuinely intersted in devoting some time to help get things going. create a pull request and lets have a conversation.



