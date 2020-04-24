# The Binary Number System #
## The Decimal System ##
We are used to using the **Decimal** or **Base 10 
**Number System.**

It is called **Base 10** because it uses ten unique digits to describe a value.

![decimals 0 to 9](./decimalOrder.png)

Even though there are only ten digits, we can indicate larger numbers by just adding more digits.

When the number 10 is reached, the next number increments and the base number starts over.

If we want to compare the decimal system to a mechanical device, we could use a dial going from 0 to 9:

![decimal illustration](./decimal1.png)

Once our first dial goes past 9, it returns to zero, and the next dial increases by one.

Similarly, if we use up all the available digits up to 99, we need to reset the first digits and add on a new one, so that 99 becomes 100.

You might notice that each time we add another digit, we increase the number by the power of ten:

1 = 10 ^ 0\
10 = 10 ^ 1\
100 = 10 ^ 2\
1000 = 10 ^ 3\
. . . \
10000000000 = 10 ^ 10

## From Decimal to Binary ##
Many systems (like computer systems) operate best with a **Binary** system. A binary system has only **two** unique values:

On/Off\
Yes/No\
True/False\
1/0

As you might guess, a device which best represents binary numbers would be a switch:

![switch illustration](./switches1.png)

Like the decimal system we normally use, binary numbers use up all of their unique values (0 and 1) before adding on a new number and setting the last.

If we have only one digit, we can only display either one or zero:

![Decimal to Binary 1 and 0](./dToB10.png)

That's easy enough. . . but we can only use 1 or 0. How are we supposed to represent  the number 2?

In decimal when we add another digit and reset the first position after reaching the number ten ("10"). In binary, we do the same thing, but instead of adding a digit every "ten", we add one every "two." It's like adding on another switch:

![Switch Diagram for Binary 2](./switchesForTwo.png)

If we want three, we just add to the end number, like in decimal.

![Decimal to Binary 2 and 3](./dToB23.png)

Similar to turning the "switch" in the 1 position back on:

![Switch diagram for Binary 3](./switchesForThree.png)

If we want to get to four, we have to add on another digit and reset the ones before it.
(so 4 = 100). For five, we can add one onto the end.

![Switch diagram for binary 5](./switchesForFive.png)

Once we reach 7 and fill up our positions, we have to continue on to 8 (1000), then eventually 16 (10000), 32 (100000), and so on.

You may have noticed by now that binary has a similar pattern to decimal when it comes to adding digits. When a decimal number adds a digit, is is increased by the next power of ten.

When a binary number adds another digit, it is increased by the power of 2.

1 = 2 ^ 0 or 1\
2 = 2 ^ 1 or 10\
4 = 2 ^ 2 or 100\
8 = 2 ^ 3 or 100\
. . . \
126 = 2 ^ 7 or 10000000 

## Converting Between Binary and Decimal ##

Converting a decimal number to a binary one can be done through a few simple steps:

1. Find the greatest power of two that is less than the number. This is your first binary digit.
2. Subtract that power from the decimal, and divide the power by two.
3. If the power is less than the decimal:
 add a 1 to the end of your binary. Subtract the power from the decimal, and divide the power by two. 
If not, add a 0 to the end of the binary, and divide the power by two.

Continue on in this way until your power is 1 or 0, and add that number to the end.

For example, if we have the number 157:

1. Our greatest power of two less than 157 is 128:
Binary: 1

2. We subtract our power (128) from our decimal (157) to get 29. We divide our power (128) by two to get 64.

Power: 64
Decimal: 29

3. Since our power (64) is greater than our decimal (29), we add a zero to the end of our binary number, and then divide our power by two to get 32.

Binary: 10
Power: 32
Decimal: 29

Our power (32) is still greater than our decimal (29) so we divide the power by two to get 16, and add another zero to the binary.

Binary: 100
Power: 16
Decimal: 29

Our power of 16 is less than 29, so we subtract it from 29 to get 13, divide our power by two to get 8, and add a 1 to our binary.

Binary: 1001
Power: 8
Decimal: 13

Our power 8 is less than 13, so we subtract it from 13 to get 5, divide our power by two to get 4, and add another 1 to our binary.

Binary: 10011
Power: 4
Decimal: 5

Our power 4 is still less than our decimal 5, so we add another 1 to our binary, subtract our decimal to 1 and divide our power to two.

Binary: 100111
Power: 2
Decimal: 1

Our power is greater than our decimal, so we add a binary 0 and divide our power down to 1.

Binary: 1001110
Power: 1
Decimal: 1

Since our last power is a 1, we add that on to get our binary.

Final conversion:
157 = 10011101
