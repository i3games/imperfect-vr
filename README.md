# Imperfect VR workshop

This is a collection of examples for my "Imperfect VR" workshop, built with A-Frame.

[The Imperfect VR Manifesto](https://github.com/i3games/imperfect-vr/blob/master/Imperfect%20VR%20Manifesto.pdf) - [Github Repository](https://github.com/i3games/imperfect-vr) - [See it online](https://i3games.github.io/imperfect-vr/)

Imperfect VR means we are not aiming for a perfect reality but will have fun in the virtual. Cheap 3D assets. Blocky textures. Weird sounds. Stumble around with a smartphone strapped to your face. Forget VR mainstream. Motion sickness will not be avoided but guaranteed. This workshop is based on the premise that everyone who can slide a smartphone into a [Cardboard](https://vr.google.com/cardboard/) can make VR experiences, even if you haven't written a single line of code before.

Imperfect VR is inspired by ["Imperfect Cinema"](http://www.imperfectcinema.com/) by Allister Gall which in turn is inspired by the essay ["For an imperfect cinema"](http://www.ejumpcut.org/archive/onlinessays/JC20folder/ImperfectCinema.html) by Julio García Espinosa.

More info about the workshop is here http://www.i3games.com/i3Games/imperfectvr.html.

## VR scenes for the workshop

* **00 Do it Yourself** - the scene for our coding exercise
* **01 Hello VR World** - result of our coding exercise
* **02 360 Image** demonstrates a 360 image
* **03 360 Video** demonstrates a 360 video. This might or might not work on phones.
* **04 Basic Scene**, based on the A-Frame documentation [Build a Basic Scene](https://aframe.io/docs/0.9.0/guides/building-a-basic-scene.html). It has animation, gaze-based interaction (looking at the cube will make it react) and sound.
* **05 Imperfect Treasures**, based on the original Google Cardboard example scene. This is similar to the last scene, but has a little bit more logic (code) in it to create a little playful experience.
* **06 The Reality of the Virtual** featuring Slavoj Žižek, Paul Virilio, Nyan Cat and more. Still a variant of or first "Hello World" scene, with more interaction, more Dubstep, more meaning, more everything.
* **07 Rabbit, Chicken, AK 47** (work in progress). This scene is my playground for more experimentation with storytelling and movement in VR. Expect it to be ... imperfect.

## Some technical and not so technical remarks

[A-Frame](https://aframe.io/) is a beginner-friendly, but capable open source framework made by people from Mozilla. It allows creating Virtual Reality experiences from HTML markup and JavaScript code. It is based on an entity-component-system architecture and has a friendly and growing community. We also use cardboard VR viewers along with our own phones.

Each example scene in this repository is self-contained and has all the files it needs in its directory structure (including fonts, images, and movies).

Everything we use in the workshop is open source. But the environment is changing and the idea of an "open web" is in danger of being superseded again by commercial monopolies.

In (utopical) theory, Virtual Reality on the Web (also called WebVR) would be an open platform on which we can build the next [Metaverse](https://en.wikipedia.org/wiki/Metaverse) together. In practice, a few gatekeepers push against it. There is not so much money to make and it is outside of their gated communities (this happen to be the same entities that run  App stores). Both Google and Apple constantly invent new and different rules about what is appropriate on the browser and implements them without asking. Google blacklists devices and sometimes tries to install "services" as soon as you open a WebVR page. Apple just decided to break WebVR completely by switching off the sensors for Safari. **If you use an iPhone re-enable it under Settings > Safari > Privacy & Security > Motion & Orientation Access.**  

This development complicates things.

While WebVR also runs on platforms like HTC Vive or Oculus Rift, the very idea behind it is that anyone can slide their mobile phone into a cardboard and off they go. You also don't need someone like Facebook to "curate the platform". In practice that does work more or less and against a certain resistance, as mentioned above.

What does this mean?

We have to become more knowledgeable in some not so exciting technical areas and spend much time with icky workarounds. Time we could rather use for creating exciting new worlds or for discussing Baudrillard's simulation theory (you decide).

A few pointers:

* You must run the scene from a web server and it must be secured with SSL (Address starts with "https", not with "http"). This means you must know how to install a SSL certificate either on your local laptop or on a public server. [Let’s Encrypt](https://letsencrypt.org) for public servers or [self-signed certificates](https://devcenter.heroku.com/articles/ssl-certificate-self) for private LANs are solutions to try. If you use [Github pages](https://pages.github.com) or [Glitch](https://glitch.com) for testing your scenes, this is done for you.
* When you open a scene on your mobile phone phone there is a mechanism to add it to the home screen and then start it from there. This can help solving some issues.
* Sometimes getting into full screen mode is still difficult.
* Scenes with audio or video have a "Start" button that must push before you enter VR. I have to check about about the new Safari thing and will try to update the component accordingly.
* To enter the fullscreen VR mode you also must push the little VR symbol. Sometimes getting into full screen mode is still difficult.
* On Android I recommend to install [Firefox](https://play.google.com/store/apps/details?id=org.mozilla.firefox&hl=en_GB), especially for older devices.

The main scene used to navigate to the individual scenes currently only makes sense for viewing the scenes on a desktop browser where you can go back and forth without interruption. The upcoming [Web XR Specification](https://immersive-web.github.io/webxr/) will hopefully allow to implement [portals](https://aframe.io/docs/0.9.0/components/link.html).

## Context and Plans

What I am aiming at are different formats - Imperfect VR jams and Imperfect VR workshops. The workshops are geared towards beginners - starting without any assumption about your background or coding experience. We go through the absolute basics, while advanced participants can get support to realize their ideas. We also discuss current politics of VR, perception, imperfection and a bit of Nietzsche.

A full day or two day workshop would be an option for teaching JavaScript, components etc.

The jams will be like game jams, people coming together for a day or a weekend and creating stuff together. The spirit of all this is captured in the [The Imperfect VR Manifesto](https://github.com/i3games/imperfect-vr/blob/master/Imperfect%20VR%20Manifesto.pdf).  

*Now make a VR!*

## Third-Party Licenses

* A-Frame: Copyright (c) A-Frame Authors, MIT License
* Uses [k-frame components](https://supermedium.com/superframe/): Copyright (c) 2016 Kevin Ngo, MIT License
* see also the README's and third-party-licenses in some of the examples.
