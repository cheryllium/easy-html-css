---
title: Color Codes Explained
lesson: 22
layout: default
---

In this section, I'll try to explain a basic understanding of how hexadecimal color codes work. You don't need to know how they work to use them, but this information is interesting for the curious! 

### Counting in Hexadecimal

Before we talk about color codes, we have to understand different number bases, because color codes are written in a base you are probably not familiar with: **base-16**. The word **hexadecimal** means **base-16**. Because humans have 10 fingers, we have evolved to count in **base-10**. But what does this actually mean?

Let's look at the number 346 as an example. Each digit falls in a certain place (ones, tens, hundreds) and tells us how many of that place there is. 346 means the sum of 3 hundreds, 4 tens, and 6 ones. But what does this have to do with base-10?

The answer? One, ten, and hundred are each powers of 10. One is 10^0, ten is 10^1, and hundred is 10^2. And the reason we are counting in powers of 10 is because we are counting in base 10. The number 348 is the sum of the following: 

- **3** times 10^2
- **4** times 10^1
- **6** times 10^0

Now, let's imagine we want to know what the number 0x346 would denote in base 16. (I will write 0x in front of all of my base-16 numbers to show that they are base 16 instead of base 10.) It's the same idea, except now we are going to multiply the 3, 4, and 6 by powers of 16 starting from the right-hand side. Instead of multiplying by 10^0, 10^1, and 10^2, we multiply by 16^0, 16^1, and 16^2. So the number 0x346 is the sum of: 

- **3** times 16^2
- **4** times 16^1
- **6** times 16^0

Which, after whipping out your calculators, we find out is 838 (in base 10!)

### Counting up to 10... I mean 16

Here's a question for you: what is the **lowest two-digit number** you can have in base 16? The lowest digit is 1, so it's going to look the same as our lowest two-digit number in base 10: a one followed by a zero. In other words, 0x10. 

This number is the sum of: 

- **1** times 16^1
- **0** times 16^0

In other words, 0x10 is equal to 16. 

Now, because we don't get to use the "tens" place (now "sixteens" place) until we hit the number 16, we actually need 16 single-digit numbers instead of 10 single-digit numbers. To solve this problem, the numbers 0-9 are the same, but then we have A=10, B=11, C=12, and so on up to F=15. 

So let's finish up this section by counting up a little in base-16. We start with 0x1, and we can count 0x2, 0x3, 0x4 and so on up to 0x9. Then, 0xA, 0xB, 0xC... up to 0xF. What's next? 0x10, 0x11, 0x12... 0x19, 0x1A, 0x1B... 0x1F... and then 0x20!

Finally, let's note that the lowest two-digit number is 0x10 (of course). What is the highest two-digit number? Take a moment to figure out what it is in hexadecimal and what value it represents in base-10.

### Additive Color Theory

A hexadecimal color code consists of six hexadecimal (base-16) digits. These digits are actually **three two-digit numbers** smushed together. The first represents the red-component, the second represents the green-component, and the third represents the blue-component. This color scheme is called RGB (Red-Green-Blue).

Already, you can imagine what the color #FF0000 is. This has 0xFF amount of red, but 0x00 amount of green and blue. So you know, just from looking at the color code, that this color is red, because it has a lot of red in it, but there is zero green or blue.

To understand anything more complicated, though, requires a basic understanding of additive color theory. In the "real world", you're used to colors behaving subtractively - that is, yellow and blue mix to make green. The reason this is called "subtractive" is because of how your eyes percieve light. 

When your eyes see something that is yellow, the object that you are looking at actually absorbs all colors EXCEPT for yellow. When you see something that's blue, it's actually absorbing all colors EXCEPT for blue. So when you mix yellow and blue, the result will **absorb** both everything yellow absorbs and everything blue absorbs. What you see is what's **left over**, which is going to be fewer wavelengths, since more are absorbed. Since it's fewer, we call this theory of color "subtractive".

However, computers work a little differently than objects in real life, because instead of absorbing light and reflecting some back, computers beam light at us directly. So when you see green light from a computer, you're looking at green light. When you see red, you're looking at red light. And when a computer shines both green and red light at you, at the same time, you are going to see both the green wavelengths and the red wavelengths. You will see MORE light instead of less, hence this theory is called "additive".

That explains why computer colors don't mix the way you expect them to. For example, in "real life", red and green mix to make an ugly shade of brown. But when a computer mixes red and green, the wavelengths combine to make yellow. Hence, the color #FFFF00 is a bright yellow (because there is red and green, and no blue.)

Finally, let's consider the difference between #FF0000 and #330000. One of these has more red in it (0xFF is greater than 0x33). Because the red component is larger, #FF0000 wil be a brighter red (there is more light being shone from the computer.)

With that said, you can probably figure out what #FFFFFF is. That's right: It's pure white, because it's the mix of all the colors together. Now, do you know what #000000 is? Hint: It's the absence of all the colors, so what color does that make?
