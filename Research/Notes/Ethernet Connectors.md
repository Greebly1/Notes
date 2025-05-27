Tags: [[Ethernet]] [[Ethernet Categories]]

The best custom Ethernet installs should be tailored to the correct cable lengths. It is also much cheaper to order hundreds of meters of raw cable in bulk. For this we must know how to crimp our own cable ends.

# Connectors
Ethernet uses 8 pin RJ45 connectors. Older telephone wires use 2/4 pin RJ11 connectors.

Just like cable, connectors also follow [[Ethernet Categories]]. For optimal performance, only use the same rated RJ45 connector for cable it is crimped to.

Also, just like [[Solid vs Stranded Core]], connectors are made for specific types. The connector will have a gold plated contact inside that indicates what type it is made for.
![[StrandVsSolidRJ45.jpeg]]

# Wiring Standard
We have two wiring standards. More will be explained after.

| PIN | SIGNAL | T568A        | T568B        |
| --- | ------ | ------------ | ------------ |
| 1   | TX+    | White/Green  | White/Orange |
| 2   | TX-    | Green        | Orange       |
| 3   | RX+    | White/Orange | White/Green  |
| 4   | TRD2+  | Blue         | Blue         |
| 5   | TRD2-  | White/Blue   | White/Blue   |
| 6   | RX-    | Orange       | Green        |
| 7   | TRS3+  | White/Brown  | White/Brown  |
| 8   | TRS3-  | Brown        | Brown        |

![[T568.png]]

In a network there are two kinds of endpoints. Computer-like and switch-like. I liken them to 'Computer Endpoints,' and 'network controller endpoints.' 
	Between the two types, their ethernet ports have flipped 'send' TX and 'receive' RX pins.
To illustrate this, imagine two blind people (both facing north) holding two continuous ropes, rope 1 in their left hands and rope 2 in their right hands. Whichever rope is sending and whichever rope is receiving is relative to your perspective. However, if you cross the ropes, they can both use the exact same communication protocol regardless of perspective.
The same is true of ethernet ports. However the 'crossing' in this case has already been done inside the ethernet port. Computers and switches interpret the pins flipped.
The cable you would use would not be crossed, these are called straight-through cables. Both ends are crimped using the same standard.

But what do you do when you need a computer to connect to a computer, or a switch to connect to a switch?
	use a crossover cable
	One end is crimped with T568A, while the other is crimped with T568B.

However, in the modern day it isn't very important to know the crossover vs straight cable distinction most ethernet controllers can probe and detect which pins are which.

# Crimping
This video showcases the process of crimping a new cable end
https://youtu.be/153ozhwcW8E
Note: It is a different process to crimp flat, slim, and ultra-slim cable jackets. See also [[Ethernet Jackets]]