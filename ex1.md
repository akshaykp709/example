# Project 5 : Piano

## {Introduction @unplugged}

**Transform your Microbit into a Piano ! **

![Description of Image](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/Piano.gif)

Turn your Microbit into a fun piano !
 
By using buttons and a buzzer, you can play different musical notes. Pressing a button changes the sound, letting you create your own tunes. It's a cool way to explore music and learn about technology ! 


## {Components @unplugged}

![Cartoon of the Rock Paper Scissors game](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/CN.png)


## {Connection @unplugged}

** Connections **

*Step 1*  
Grab your *Microbit, **Breadboard* and move to next Step ..
![Image 1](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S1.png)

## {Connection @unplugged}

*Step 2*  
Place 5 Pushbuttons on the breadboard as shown below  
![Image 2](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S2.png)

## {Connection @unplugged}

*Step 3*  
Place 5 1kohm Resistor one by one an show in the below steps
![Image 3](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S3.png)

![Image 4](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S4.png)

![Image 5](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S5.png)

![Image 6](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S6.png)

![Image 7](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S7.png)

## {Connection @unplugged}
*Step 4*  
Connect the *3v* pin of Microbit to the Resistor as shown
![Image 8](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S8.png)

## {Connection @unplugged}
*Step 5*  
Connect the Pushbutton Pins One by one as shown below in an Series connection  
![Image 9](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S9.png)

![Image 10](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S10.png)

![Image 11](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S11.png)

![Image 12](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S12.png)

## {Connection @unplugged}
*Step 6*  
Connect the Pushbutton series connection with Microbit Pin *P0*
![Image 13](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S13.png)

## {Connection @unplugged}
*Step 7*  
Add a resistor as Shown
![Image 14](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S14.png)

## {Connection @unplugged}
*Step 8*  
Coonnect the Onter end of the resistor witht the *GND* of ** Microbit**
![Image 15](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S15.png)
Turn your micro:bit into a *Rock Paper Scissors* game that you can play with your friends!

## {Start Programming @unplugged}
Connect you *Microbit* with your Computer
![Lets Start Programming Image](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/LSP.png)

 

## {Step 11}

First we need to make a variable to keep track of value read from *P0*.   
A variable is a container for storing values. Click on the `||variables:Variables||` category in the Toolbox. Click on the *Make a Variable* button. Give your new variable the name "Value" and click Ok.

![A animation that shows how to create a variable](https://raw.githubusercontent.com/Edusharks/Microbit-Basics-Resource/main/project9%3APiano/S0.gif)

blocks
basic.forever(function () {
	
})


## {Step 12}

Click on the `||variables:Variables||` category in the Toolbox again. You'll notice that there are some new blocks that have appeared. Drag a `||variables:set Value||` block into the `||Basic: forever||` block.

blocks
let Value = 0
basic.forever(function () {
    Value = 0
})




## {Step 13}

Click on the `||math:Math||` category in the Toolbox. Drag a `||math:pick random||` block and drop it into the `||variables:set hand||` block replacing the number 0. Now when we shake our micro:bit, the variable hand will contain a random number between 1 and 3.

blocks
let hand = 0;
input.onGesture(Gesture.Shake, function() {
    hand = randint(1, 3)
})


blockconfig.global
randint(1, 3)


template
basic.forever(function () {
	
})
