# Keyboard2022-SplitSpaceBar

Repository contains the necessary files for a brand new keyboard idea I had. 

## Tenets

1. **High Quality**
    * Keyboard should be designed as the keyboard to end all keyboards (for me anyway)
1. **Utilitarian**
    * Keyboard is designed specifically for an office environment
1. **Portability**
    * Keyboard is designed to be as portable as possible since it could commute with me to work
1. **User Friendly**
    * Keyboard should be easy enough to use for someone not acquainted with it (like a coworker trying to help with something)

## Design Thoughts
After using the keyboard built in the [previous keyboard project](https://github.com/JonathanGWesterfield/Keyboard2019), I noticed there were still some improvements to make. 

Specifically, I only used half the space bar (I only hit space with my right thumb) and thus, a new can be used for the half I don't use. With this new key (I'll refer to it as fat function), I can add a new function key to access the function layer. 

On this function layer, I can add the numpad to it. Since I would be using my left thumb for function, this numpad could be put on my right hand (I'm right handed). This removes the left-handed number pad layout on the [previous keyboard project](https://github.com/JonathanGWesterfield/Keyboard2019). While the left handed numpad actually worked extremely well (the left hand somehow uses the same muscle memory as the right hand), it added to the length of the keyboard, which went against the _Portability_ tenet.

### Problems
In the last design, I was able to integrate a teensy controller directly into the PCB by putting all of the pins in between the switches under the space bar. There was a large gap I could use. You can see this in the PCB files, specifically in the PCB layout file.

This split space bar keyboard is more dense and uses up that space. 

I need to figure out how to wire the teensy. Thinking of using a ribbon cable, and having the teensy be mounting somewhere in the keyboard case. 

This still poses a problem of figuring out where I can mount an adapter for the ribbon cable though.

#### Alternatives to solve the main problem
I can see 3 ways to get around this

1. Figure it out
1. Directly wire each pin to the pcb
    * Pros: Relatively simple and straight-forward
    * Cons: Crude, disgusting, hard to maintain should I need to lift/disconnect something
1. Don't use teensy and mount a microcontroller directly to the keyboard PCB
    * Pros: Elegant and extremely durable. Small controller should be able to fit under the space bar
    * Cons: Hard AF. I'm not comfortable with microcontrollers so it would be a huge and time consuming learning curve. Not to mention I'd have to figure out which micro controller to even use

## Tools
* [Keyboard Layout Editor](http://www.keyboard-layout-editor.com)
* [Keyboard Plate CAD Drawer](http://builder.swillkb.com/) 
* PCB Editor: Eagle
