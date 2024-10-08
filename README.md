# Cantabile for Beginners

## Welcome!

Hello and welcome to the Cantabile community!

[Cantabile](https://www.cantabilesoftware.com/) is a powerful tool for performing music with software instruments and effects, and there is a very active group of people here who use it during live performances and are happy to help new users getting to grips with Cantabile. 

While Cantabile is very powerful, it is also a complex piece of software - learning Cantabile is a bit like learning an instrument. You’ll have to learn some foundations before you can really use Cantabile for your specific application. You will have to invest some time and be serious about understanding how it all works - Cantabile is not a simple “click-and-play” solution.

There are a number of topics that are frequently asked by new users of Cantabile in the [Cantabile forum]([https://community.cantabilesoftware.com/](https://community.cantabilesoftware.com/)); to avoid having to answer these questions all over again for every new user, this is an attempt to create a first foundation of knowledge that will enable you to take your first steps with Cantabile, and also to have a common basis of reference when you come to the forum to ask your question.

This will by no means be the tell-all-and-end-all manual for Cantabile, but once you work your way through this guide, you should be able to get going, using Cantabile for most of the usual scenarios, and also have the knowledge to find your own way, building on that to get to the more sophisticated things with the available resources.

This document has been created on the basis of my learnings getting started and more experienced with Cantabile over the years, and prioritized by the topics of the questions I frequently read in the [Cantabile forum](https://community.cantabilesoftware.com/){:target="_blank"}. 

I have invited other experienced users to contribute to this article. All contributors will be credited explicitly here - thanx in advance for your help!

# Table Of Contents

1. [What Cantabile does](#what-cantabile-does)

2. [What you need](#what-you-need)

3. [What you should know before starting](#what-you-should-know-before-starting)

4. [The Cantabile Fundamentals](#the-cantabile-fundamentals)
   
   1. [Basic setup](#1-basic-setup)
   
   2. [Navigating the user interface](#2-navigating-the-user-interface)
   
   3. [Building Songs](#3-building-songs)
   
   4. [Creating Layers and Splits](#4-creating-layers-and-splits)
   
   5. [Working with instrument / effect presets](#5-working-with-instrument--effect-presets)
   
   6. [Using song states to change configurations quickly](#6-using-song-states-to-change-configurations-quickly)
   
   7. [Bindings](#7-bindings)
   
   8. [Racks](#8-racks)
   
   9. [Setlists](#9-setlists)
   
   10. [Pre-loading](#10-pre-loading)
   
   11. [Media Players](#11-media-players)

5. [Advanced Topics](#advanced-topics)

6. [When asking for help in the Forum](#when-asking-for-help-in-the-forum)

# What Cantabile does

Cantabile is a “VST host” - what does this mean? Essentially, Cantabile is a piece of software that allows you to “play” VST plugins in a live context. VST plugins are typically used in DAWs (digital audio workstations - essentially music production software), and they come as “instruments”, which generate sounds (e.g. a piano), and “effects” which process sound passing through them (e.g. an equalizer). VST plugins can’t run on their own - they need a “host” that they plug into - usually, this is a DAW. Cantabile is a special kind of host to allow you to play these plugins live instead of using them in a recording and production context. You “play” these instruments by sending MIDI signals to Cantabile from an external controller keyboard and letting Cantabile create and process the sounds.

If you are shaking your head at this point and you have no clue what all this is, then Cantabile probably isn’t for you - you need to have a working knowledge of VST plugins (and MIDI in most cases)  to use Cantabile. 

So now we have this out of the way: Cantabile allows you to “play” VST instruments in your PC - usually via MIDI commands from an external controller keyboard (masterkeyboard, synthesizer). Cantabile lets you create complex “chains” of instrument and effect plugins to shape your sound, and it lets you switch between different configurations of these instruments and effects easily and quickly, so that you can e.g. jump between a clean piano sound and a distorted organ with lots of delay with the touch of a button.

While there are also other use cases of Cantabile (e.g. using Cantabile as a “guitar amp”, feeding a guitar signal through an amp simulation or using Cantabile to process vocal signals for a podcast), we will focus this Beginner’s Guide on the base case of playing VST instruments with an external controller keyboard. Keep things simple…

# What you need

- a reasonably powerful PC → there are multiple discussions on the forum about reasonable PC (or laptop) specifications; best use the search function for this  
- an audio interface and a way to hear its output (speakers or headphones). It is typically not advisable to use the on-board audio devices of laptops or PCs for live VST use, both from a sound quality and from a latency perspective (more on latency later)
- a MIDI controller keyboard or synthesizer (more on special cases later). There are different ways to connect this keyboard to your PC - directly via USB or through a dedicated MIDI interface and special "DIN MIDI cables". More on this later as well.

# What you should know before starting

Cantabile is a pretty sophisticated piece of software, and it builds on some principal technologies of the digital audio world. We can’t explain all of these in this document, so we will expect new users of Cantabile to have a working knowledge of:

- digital audio processing via VST plugins
- the MIDI protocol (commands, notes, controllers, etc)
- Audio and MIDI interfaces and how to configure them

If you have some experience with recording and producing audio and using VST instruments in a DAW (digital audio workstation) on a PC, you should have sufficient experience to be fine with Cantabile as well.

Some articles on fundamentals for absolute beginners:

- [what is a VST](https://emastered.com/blog/what-is-a-vst)?
- what are [VST plugins](https://www.samplesoundmusic.com/blogs/news/what-are-vst-plugins-a-beginner-s-introduction) and how do I use them?
- [what is MIDI](https://nektartech.com/article/blog/all-you-need-to-know-about-midi/) and how to use it

# The Cantabile Fundamentals

Before coming to the forum and asking “how do I …”, you should have a working knowledge of the fundamentals of Cantabile. There is no way around learning the basics yourself, which will always involve a bit of trial and error. But there are some great resources available, which we will point you to in the following sections.

Overall, the best way to learn about Cantabile are the [Guides section](https://www.cantabilesoftware.com/guides/) of the Cantabile website and the excellent [foundational videos](https://www.youtube.com/playlist?list=PL1PQg6oOZdtDDw6MME0B12p0kCs3LAHbx) produced by Brad Robinson, the mastermind behind Cantabile. 

There is also an excellent “real life” [Cantabile Guide](http://www.xfactory-librarians.co.uk/Downloads/CantabileGuide.pdf) by Derek Cook - he describes his live setup with Cantabile in detail. Some of that content may only make sense to you once you have progressed in your knowledge of Cantabile, but it can be very useful to see how it all fits together.

## 1 Basic setup

Before starting to build your songs, you’ll have to install and configure Cantabile. Please watch the first 14 minutes of Brad’s [first video](https://youtu.be/FvUL2rte-YY) before - this will help you enormously. First: download and install Cantabile

- You’ll need to decide which license to use - best start with the free “Lite” version, and once you get to the more sophisticated aspects of Cantabile, you can start a trial of the more powerful “Solo” and “Performer” editions
- Once Cantabile is installed, you’ll need to configure your audio and MIDI connections. 
- You’ll also need to configure where you want to save your Cantabile-related files, and the location of your VST plugins
- Note: there are two fundamental plugin architectures: 32 bit and 64 bit. A 32 bit host can only load 32 bit plugins, a 64 bit host only 64 bit plugins (well, there are tricks to work around this, but we’ll not go there in a Beginner’s guide). There are actually two versions of Cantabile (32 and 64 bit) installed, and you can choose which one to start by default. You need to be sure you are configuring Cantabile with the correct path to your plugins (32 bit or 64 bit). 

Here are the relevant guides sections: [Installation](https://www.cantabilesoftware.com/guides/installation), [Getting Started](https://www.cantabilesoftware.com/guides/gettingStarted).

Expert tip: Do yourself a favor at this time and do NOT use “hardware” names for your audio or MIDI ports (e.g. “Scarlett 2i2”, “M-Audio Oxygen”), but rather stay with “logical” names like “Main Keyboard”, “Upper Keyboard”, “Main Output”, “Monitor Output” and the like. You may want to change your hardware in a year or two without having to re-work all your Cantabile songs… More on this later in a dedicated section.

### Latency and audio drivers

To use VST instruments and effects live, it is key to have a setup that allows you what is called “low audio latency”. So what is this beast called “latency”? 

Audio latency is essentially the time it takes for audio signals to be processed before they get heard. When audio applications process signals, they don’t do this sample-by-sample but in “chunks” of samples. So an effect takes a number of samples - this is called a “buffer”- from the audio interface, performs a number of calculations on them and then provides a modified buffer as its output. Same with an instrument: it takes MIDI notes or other events as its input and provides a buffer of output. This is then handed over to the next plugin in the chain, which again processes it and hands it on, until the end of the chain. Then this buffer is handed over to the audio interface for output. So all audio processing happens in cycles, and the length of these cycles is determined by the buffer size of your audio interface.

This is less important for DAWs, since their purpose is recording and re-playing of recorded stuff, but when you want to use VST instruments and effects live, you want snappy reaction times between hitting a note and hearing the sound. So you’ll want to configure your audio interface for the smallest buffer size you can get away with. But there’s a limit: your PC needs to do all its audio processing within the time it takes for the audio interface to push out one buffer, so that a new buffer is ready when the audio interface comes back for the next one. If the calculations are too complex (i.e. your instruments and effects are too CPU-hungry), the new buffer will not be ready in time, and you’ll have audio dropouts - typically crackles and distortions of your output signals.

Typical buffer sizes in well-configured audio systems will be somewhere between 128 and 256 samples - beyond that gets a bit sluggish to play. Some of us have managed to get their buffers as low as 64 samples, but that will only work reliably on powerful machines with not-too-complex setups.

The selection of audio drivers is important in your audio setup. Most decent audio interfaces provide drivers supporting the ASIO standard (“ASIO drivers”), which enables efficient low-latency communication between Cantabile and the audio hardware and also allows you to configure buffers and thus latency directly. If your audio interface provides such an ASIO driver, you should definitely use that. Dedicated ASIO drivers are usually the most efficient way to address your interface, and they will help you get the best performance from your setup, i.e. you’ll get the lowest latency out of your interface. 

 If your audio interface doesn’t have such a driver - or if you are trying to use Cantabile with your on-board hardware, you might be able to either use WASAPI (a Windows mechanism to connect to the audio interface) or a special driver called ASIO4ALL. ASIO4ALL allows you to use ASIO with audio interfaces that don’t have specific ASIO drivers. It can be a bit fiddly, but it can definitely help you work with interfaces that don’t provide ASIO drivers.

Important: WASAPI only gives you output capability, so playing VST instruments via MIDI will work, but processing audio input (adding effects to a microphone signal or playing a virtual guitar amp) will not work with WASAPI.

Another important thing to know: you can only use one ASIO driver at a time, which means you cannot combine multiple interfaces in your setup (e.g. to get more output channels). So choose your audio interface according to all your input and output needs. Yes, there are exceptions to this, and people have managed to work around this restriction, but for the purpose of a Beginner’s Guide, take this as a rule: use only one audio interface in Cantabile!

### Optimizing your PC for audio

Beside the selection of your audio interface and drivers, there are numerous factors affecting the ability of your PC to deliver low-latency audio performance without crackles and drop-outs. Brad Robinson has compiled an excellent eBook that explains what is important in selecting and configuring a PC for optimum audio performance. You can download this eBook for free at [https://www.cantabilesoftware.com/glitchfree/](https://www.cantabilesoftware.com/glitchfree/)

### MIDI connection

To connect your MIDI keyboard / controller to Cantabile, there are usually two options:

1. These days, most keyboards and controllers are connected to your PC with USB cables and provide their own MIDI driver to Windows. You may have to install specific MIDI drivers for Windows to recognize these devices, others are what is called “class compliant”, which means that Windows will automatically recognize them. After installation, Cantabile will find your Controllers as individual MIDI devices.

2. A number of keyboards and controllers also give you the option to connect via “classic” DIN cables (the round ones with five pins). To use these, you’ll either need a dedicated MIDI interface or use the MIDI ports on your audio interfaces (if your interface has them). Now your keyboards will not show up individually in Windows, but you’ll have to remember which port of your MIDI or audio interface they are connected to.

There are some advantages and disadvantages to both:

- USB MIDI has a far higher data rate, so if you are creating a lot of controller data, USB MIDI is far less likely to “hiccup”
- USB MIDI requires a separate USB port for every device and doesn’t always play nice with USB hubs
- DIN MIDI is slower, so if you’re about super-precise timing of a lot of data, will not be your first choice
- DIN MIDI allows you to switch out devices easily - just unplug the old keyboard and plug in the new one without having to worry about drivers and configuration. It is also “hot-plug”, so unplugging and re-plugging a device is unproblematic.
- You can have 4- or 8-port MIDI interfaces using just one USB port, which can be useful when USB ports are scarce

Overall, you’ll have to make your own decisions how to best set up your MIDI connectivity - ask around in the forum if you have specific questions!

### Virtual vs. physical ports - audio and MIDI

One thing that frequently trips up new Cantabile users and also comes back to haunt them years later is the logic around its audio and MIDI ports. 

Cantabile addresses audio and MIDI hardware at two levels: 

- a higher "abstract" level of "logical" input / output ports that get used with Cantabile's songs

- a lower "physical" level of the technical devices that are actually connected to your PC and that you typically see in your system configuration. These "physical"" devices need to be assigned to your "logical" devices so that you can actually use this

This sounds convoluted at first, but the advantage of this two-layered logic is that you can create your songs based on the _function_ of an input/output port and not based on the _technical device_ attached to your PC. If you want to use your Cantabile songs on a different PC with different hardware, all you need to do is install Cantabile on that PC, re-create your logical ports, assign the hardware ports to your logical ports, and all your songs will work nicely.

Also, when you change any part of your hardware setup in a few years (once G.A.S. hits again), you simply change the assignment of hardware ports to logical ports and you won't have to change anything in your ports.

So there is one iron principle (ignore it at your peril!): **use functional names instead of technical names for your audio and MIDI ports**

- "Main Keyboard", "Second Keyboard", "DrumPad" instead of "Motif XF 6", "Keystation 49", "nanoPAD2"

- "Organ Out", "Piano Out", "Monitor Out", ... instead of "Babyface 1/2", "Scarlett 2i2 1/2" etc

## 2 Navigating the user interface

To understand the user interface, there is a whole section in the user guide: [see here](https://www.cantabilesoftware.com/guides/mainWindowControls). But this can be a bit complex to read un-prepared - it is usually easier to first watch Brad's [first video](https://youtu.be/FvUL2rte-YY). By watching Brad operate Cantabile, you will get the idea of the key parts of the Cantabile window.

As a beginner, your starting point should be the "Routing View" - the big area at the heart of Cantabile's window. This is where you insert plugins for instruments and effects and where you create Audio and MIDI connections between these plugins in order to send MIDI commands (key presses, controller moves) to your instruments and to send the resulting audio from your plugins through others (e.g. an equalizer or a reverb) and then on to the output ports.

![](Pictures/main-window.png)

The main window has three view modes (at least in the full version; not all modes are available in the "smaller" versions). For now make sure that the "Routing" view is active

![](Pictures/routing-view.png)

### Table View vs. Wiring View

There are two ways the routing window can be displayed: there is the "table view", which displays your song as a table of horizontal lines, with individual lines for every plugin in your setup and "folded-in" lines for all the connections between them (we call them "routes"). Routes can be shown by "expanding" the plugin line and hidden by "collapsing" the plugin line using the "+"/"-" button at the left.

![](Pictures/basic-song.png)

The "wiring" view is a more graphic view that may help you understand the flow of audio and MIDI in a setup better. But this also means that less information on the state of a plugin or a route is shown - you'll have to decide which view works better for you.

![](Pictures/wiring-view.png)

There is a dedicated page in the Guides section explaining how to use the Wiring View - [see here](https://www.cantabilesoftware.com/guides/routingDiagrams).

For the rest of this guide, however, we will use the Table view - some configurations are just easier to explain in this view.

## 3 Building Songs

The first stage of using Cantabile is building simple songs, which contain an instrument plugin and maybe one or two effects plugins to process the output. You can start out with an instrument and an effect you know well (maybe a nice reverb?) and connect them to make Audio and MIDI flow between them.

Routes are the fundamental thing that connects everything in Cantabile - MIDI routes connect MIDI inputs (e.g. from your keyboard controller) to VST instruments; audio routes connect instruments to effects or outputs, or effects to other effects or to outputs.

Now is the time to watch the second half of Brad’s [first video](https://youtu.be/FvUL2rte-YY) - and you can learn all about routes in Brad’s video [here](https://youtu.be/1L5I-gialKU)

The relevant Guides sections are [Ports and Routes](https://www.cantabilesoftware.com/guides/portsAndRoutes) and [Working with Plugins](https://www.cantabilesoftware.com/guides/workingWithPlugins) - work your way through them and things will be pretty clear!

Now start working with your favorite plugins and build your first own setups. Once you have created a setup that you like, you can save it - this is called a “song” in Cantabile. Usually, you create a "song file"" for each of the songs you play (if you want to create specific sound configurations for every song), but there are also users who use just a few basic configurations that they use across a number of songs, e.g. “piano & strings”, “organ”. We’ll also call these “songs”, OK?

Here is an example of a very basic song: MIDI input from your keyboard routed to an instrument plugin (in this case a DX7 emulation called "Dexed"), creating audio output from Dexed. This audio output is then routed through an effect plugin (a reverb from the kiloHertz bundle) where it gets some reverb added to it. The result of this is then sent out to the output port so you can hear it.

![](Pictures/basic-song.png)

This is just a simple linear effects chain, with a single "line" from MIDI input to audio output. But songs can become far more complex - any input port or plugin output can be sent to multiple destinations by just adding more routes. Also multiple routes can be sent to one single destination; Cantabile will take care of the mixing automatically when you e.g. send multiple plugin outputs to "Main Speakers" - there is no need for an explicit "Mixer Block" to mix the signals together; Cantabile will do that for you. The same applies for MIDI routes: Cantabile will automatically merge the MIDI data from multiple routes at their destination, so you can route MIDI from multiple keyboards or controllers to the same plugin.

Now start constructing your own songs and get a feel for Cantabile - come back to this guide once you feel comfortable with this.

## 4 Creating layers and splits

Where Cantabile excels is creating layers and zones from multiple instruments - you can go absolutely wild stacking and mixing multiple sounds for that monumental sound or creating as many split zones (overlapping if need be) as your keyboard has keys.

### Layering

To layer the sound of two plugins, simply create TWO routes from your MIDI input (let's say: Main Keyboard) and connect them to two different plugins (that are both routed to your output). Now, when you play a key, this note will be sent to both plugins. Cantabile will automatically mix the output from both plugins; no need to worry about this. To change the mix between the sounds, simply adjust the Gain for the individual plugins. 

To layer even more, simply add more routes and more plugins...

You may want to transpose individual layers (e.g. to get these high silvery strings over your piano). Of course you can transpose the sound your plugin makes, but the easiest way to do this is simply transpose the MIDI notes sent to your plugin. 

The key to this are the properties of your routes - when you right-click any MIDI route and select "MIDI Route Properties..." (or you click the "Control" column of the route line; the part that initially says "Omni"), you get to a big settings page that allows you to make all kinds of settings to filter and modify the MIDI notes getting forwarded to your plugin:

<< picture>>

Use the "Transpose" setting to change the MIDI notes sent to your layer - the Transpose setting is displayed in the format "octaves.semitones", so transposing all notes up by an octave means "1.0".

### Keyboard Splits / Zones

For this, start as with layers and create your routes from your keyboard to multiple plugins, then use the Midi Route Properties, now with the "Note Range": by using the "Lowest Note" and "Highest Note" Boxes, you can filter the range of notes that will be sent to your plugin. So if you select 60 to 72 here, only the notes of the octave starting with "middle C" will be sent to that specific plugin. So you have created a 1-octave zone that is sent to this one plugin. 

Make similar settings for your routes to your other instruments, and you've created multiple keyboard zones. These can be fully separated or overlap - this is all determined by the key ranges you set for your routes.

With splits and zones, it will often be necessary to transpose some of your zones (maybe that top octave you only use for a quick brass phrase). Use the Transpose setting in the MIDI Route Properties for that.

More details on the MIDI Route Properties: see the [guide for this topic](https://www.cantabilesoftware.com/guides/midiRoutes).

### Advanced Layering Techniques

If you want to create a "**velocity layer**", with individual instruments only playing for a certain velocity range (e.g. add a crash cymbal on very hard hits of a bass sound), you'll need to use MIDI filters on that route. 

*Note: This is a feature that requires at least Cantabile Solo.*

To create a velocity filter on a route, click the "funnel" icon on the MIDI route - this will show you the MIDI filter page. Here, insert a "Velocity Gate" filter and set it to focus on the range of velocities that you want to play this instrument on. Select "Suppress out of range notes" so that all other notes don't play, and you're done.

See the [Filters Section](https://www.cantabilesoftware.com/guides/midiFilters) of the Guides for more details.

Another useful technique is to **layer an instrument with itself** - simply create two or more transposed routes to the same instrument. Easily create octaved brass phrases or instant chords using this technique.

## 5 Working with instrument / effect presets

## 6 Using song states to change configurations quickly

## 7 Bindings

What are Bindings? Essentially they are Cantabile’s mechanisms for all kinds of automation or remote control. They allow you to

- control parameters of your plugins via your MIDI controller

- remote-control aspects of Cantabile via MIDI (e.g. go to next song state)

- Do things automatically when certain “events” happen in Cantabile (e.g. send MIDI to an external device when a song loads, or automatically setting the Leslie speed of your virtual Hammond when changing song states)

- and lots more…

Bindings are version-dependent: you don’t get them in Cantabile Lite; Cantabile Solo contains a subset of bindings (it allows you to control things via MIDI, but not automate via “events”); you’ll need Cantabile Performer for the full set of capabilities.

You find your bindings in Cantabile’s “Bindings” tab:
![Bindings tab](Pictures/cantabile-bindings-tab.png)

You can also go to this tab with the keyboard shortcut CTRL-D

All bindings have a “source” and a “destination”. The source tells Cantabile what to listen for, and the destination essentially tells it what to do when this source event occurs.

Sources are generally three categories:

- MIDI events that arrive from a MIDI port (notes, controllers, …)

- Parameter changes from VST plugins

- Events in Cantabile (song load, state load, etc)

Destinations are similar: you can

- send MIDI to MIDI ports

- control VST plugin parameters

- initiate actions within Cantabile (go to specific songs in a setlist, change song or racks states, start media player playback, etc.)

Now that you are armed with this knowledge, it is the time to watch the [video on Bindings](https://youtu.be/Czc9PU7opSs) and read the [Bindings chapter of Brad’s user guides](https://www.cantabilesoftware.com/guides/bindings) - this will give you all the nitty-gritty detail on how to create and manage bindings. 

One important aspect: when it comes to MIDI sources, you’ll have to learn about control changes (CC): since CC commands can be used both for “triggers” (like pressing a button) and for “controllers” (pots and sliders), Cantabile needs to know how to deal with them. Mostly, Cantabile will pre-select a useful option based on the destination you select, but it is essential to know some key options:

- Controller - this captures the value of the controller (0..127) and translates it to the target. This way, you can e.g. use a slider on your MIDI controller to change the cutoff frequency of a filter. Or you may want to use the mod wheel (CC1) to control the Leslie speed of a Hammond plugin. You can customize the range and the “curve” of this control on the destination side of a binding

- Controller (Button) - this interprets the CC input as follows: when the CC value first crosses >=64, the binding recognizes this as an event (or a “trigger”). These triggers can now initiate actions on the destination side of a binding, like starting media player playback or changing to the next song state. Important: after triggering the event, this source waits for a CC value <64 before it can be triggered again. So this type of binding source will work for sliders and pots (it will trigger when they cross the 50% mark from low to high) and it will work for buttons that send e.g. 127 when you press them and 0 when you release them. But it will NOT work for buttons that only send MIDI when you press them - it will react exactly ONCE and then wait endlessly for the “release” signal that never comes… That’s why you’ll need the next option:

- Controller (No-Edge Button): This binding will “fire” on ANY CC value >= 64. As such, it is exactly the binding you need when you want to start actions by pressing a button that only sends values when pressed, but not when released. You definitely DON’T want to use this to trigger events with sliders, pots or wheels: this will create a ton of triggers once the slider is above the threshold. 

A final note: bindings can exist at multiple levels: 

- you will probably use bindings at song level first - to use MIDI controllers or song states to control your plugins or to automate things

- racks (next chapter) can also have bindings embedded. This can be very helpful to do things inside a rack based on input that rack receives through its MIDI input. But bindings can also be used e.g. to initialize parameters within a rack whenever a song is loaded

- if you have certain bindings that aren’t song-specific (e.g. if you have buttons that you want to use to step forward/backward between songs), there is a special place for them: the Background Rack. We’ll also get to that in the next chapter.

## 8 Racks

### The Background Rack

## 9 Setlists

## 10 Pre-loading

## 11 Media Players

# Advanced topics

## 1 Using the Controller Bar

## 2 MIDI tempo and synchronization

## 3 Processing audio input

- e.g. playing guitar through Cantabile

- using audio inputs - need for ASIO drivers

- respecting round-trip latency

## 4 Cantabile for streaming and conferencing

- relevant videos on voicemeeter by Terry Britton

## 5 Using Show Notes

## 6 Multiple configurations

# When asking for help in the forum

Following this guide, you should have a good knowledge of the relevant aspects of Cantabile, but there will be times when you get stuck, or when your specific situation requires something that someone else on the forum might know - that’s the time to reach out to your brethren at the Cantabile Community.

There is a bunch of really knowledgeable and experienced people out there, who are usually very friendly and helpful, but there’s a couple of things to keep in mind when asking questions in the forum:

- be polite and friendly - no ranting, swearing or personal insults, and NO SHOUTING, PLEASE

- search first - a lot of questions can be addressed by finding answers already given in the forum

- be as specific as possible - use screenshots to illustrate your specific use case and give as much detail on your configuration as may be useful for others to understand. “I’m not getting any sound” is not really helpful for others to diagnose the problem…

- The universal language on the forum is English - don’t worry if your native language isn’t English; there are people from all over the world here, so nobody is going to flame you on grammar or syntax. There are also tools like Google Translate or DeepL that can help you create your posts in English or translate English posts to your native language. If you post in another language, you will drastically limit the number of people who can help you.

- The same applies to screenshots: it will be difficult for others in the forum to understand your specific problem if you are using a localized version of Cantabile to create your screenshots. It may be a good idea to keep Cantabile set to English if you plan to interact with the forum on a regular basis.

- please keep in mind that people on the forum are helping you on a voluntary user-to-user basis - you have no claim on their time and energy, so be respectful of that
