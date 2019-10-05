##Problem:
For my family's mailbox rentals & related services business, manual mail-sorting is a natural bottleneck. Every morning, several batches of our customer's mail is dropped off by the post office and it is our duty to sort and subsequently place the mail into the mailboxes. On a table, mail is bundled into ~10 categories by mailbox numbers ranging from 80 to 900. This task takes up to 90 minutes and becomes quite tedious. Thus, this is a worthwhile and automatable process to tackle anytime I'm overseeing the business.

Goals:
Using minimal capital (<= $100) create a prototype, both hardware and software, of a mail-sorting robot.

Learning Goals:
Input/Output Communications, Arduino, Processing, Circuits, Servo Motors and Machine Learning.

Concept:
Limited to a 65" x 23" space, the crude idea was to have a unidirectional machine to drop mail on either side of its platform.
1. Take picture of envelope
2. Read only #
3. Travel on rail
4. Drop off mail on either side depending on number (or multiple in one sweep)
5. Reset
6. Repeat

![1](https://user-images.githubusercontent.com/42861174/66092295-6532b380-e540-11e9-82d3-ac05c5bf04f9.jpg)

Actions:
After developing a concept, I purchased an Arduino Uno kit, several metal, continuous Servo motors, and a 16 Channel PWM/Servo Driver IIC Module. I learned A LOT from this YouTube video:

https://www.youtube.com/watch?v=kUHmYKWwuWs

I followed through the built-in Arduino examples and started messing around with a circuit board, and a potentiometer.

![20180630_190855](https://user-images.githubusercontent.com/42861174/66090645-31a05b00-e539-11e9-9e4e-02d72b20647f.jpg)

I attached the motor and played around with that as well. My next goal was to create a mechanism for the machine's platform to travel. 

A beyblade ripper and rip cord quickly came to my mind. But that was soon discarded when the costs to 3D print a sufficiently long cord exceeded my budget. 

![3](https://user-images.githubusercontent.com/42861174/66092299-6663e080-e540-11e9-8b4c-c6d10b074075.jpg)

I quickly jumped to build the physical structure for the machine. To limit my costs, I only used items that I found throughout the business. I used boxes, cardboard, tape, and newspaper. I used a screwdriver on the opposite side as a pivot point and electrical tape as travel cord. 

![8797644993090097300](https://user-images.githubusercontent.com/42861174/66091173-8e9d1080-e53b-11e9-81bc-7048e00f03b8.jpg)

![5](https://user-images.githubusercontent.com/42861174/66091505-e5efb080-e53c-11e9-8c39-281fae5c5bf3.jpg)

Cord tension was a slight issue but my setup was temporary and it worked! Next was to work on the code for reading the envelopes. 

![6](https://user-images.githubusercontent.com/42861174/66091510-e7b97400-e53c-11e9-832e-e3560512192a.jpg)

Potential challenges: The envelopes vary (pictured) and it was necessary to extract ONLY the mailbox numbers. Orientation of the envelope (if placed backwards or upside-down) was important and a unknown/redo pile may be required.

![4416377185118805301](https://user-images.githubusercontent.com/42861174/66090675-48df4880-e539-11e9-993b-9b49bad32c12.jpg)

![2140152601971035198](https://user-images.githubusercontent.com/42861174/66090677-4b41a280-e539-11e9-95c2-57fe9d0bd54a.jpg)

...tbc
