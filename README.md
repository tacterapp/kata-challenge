# 💻 Tacter's code challenge

We've prepared for you a repository with a kata from [rviewer.io](https://go.rviewer.io/dev-build-a-wall/) in order to 
showcase your skills and knowledge. **We've added a few extra house rules**, so keep reading this README and not the 
original one.

Start by cloning this repository. You can commit your changes to the main branch locally but once you've completed the 
task you must create a [git patch](https://www.git-tower.com/learn/git/faq/create-and-apply-patch/) and send it over to 
us via email instead of pushing to remote.

## 📚 Challenge description

The aim of this challenge is to create the strongest wall of all time! You will have to combine bricks, in a proper way, 
to avoid instability.

### ⚙ How it works

You should implement a CLI application that receives **at least** 2 arguments and represents the created wall in ASCII.

You will need the following mandatory parameters:

- Number of rows: The number of rows of bricks the wall needs. This will make the wall taller or smaller.
- Number of bricks: The number of bricks you have to use on each row to represent the wall. This will make the wall 
longer or shorter.

### 🎨 How to represent your wall

To represent your one-and-only creation you have to use the following elements:

👉 ■■: A full brick (2 of ■). The bigger brick for the wall.

👉 ■: Half a brick. The smallest unit.

👉 |: Mortar. The cement between each brick on the same row.


#### 🧱 How to build a strong wall

Any builder knows that if you just put a brick over another, your wall is going to fall down as you turn your
back!

To build a strong wall you have to follow these considerations:

* There has to be a mortar (|) between each brick (half or full) on the same row.
* Bricks cannot be aligned vertically with the bricks of the row above or below it, to provides more stability.

## 🎯 Objective

We are aware that this challenge could be solved easily by just focusing on the algorithmic part, even with a
single function, in quite a clean way.

**However**, that is not what we are looking for. We want to see how comfortable you are around **SOLID**, 
**design patterns** and **clean architectures**.

This is not to say that you should cram as many design patterns as you can find around the internet like
one (not me, of course) might do for a particularly boring software design college assignment. Use your better judgment 
and implement a solution that **makes sense**, but that considers the above points.

To help you with this, we bring up some scenarios that your code should be prepared to handle (but the sky is the limit):
* more than two brick sizes (ie: ■■■, ■■, ■) while respecting the overlapping rule
* receiving the different brick sizes as parameter  (keep it dynamic)
* receiving the icon (UTF-8 emoji or ASCII symbol) for the brick and mortar as parameter
* using different brick icons for odd and even rows
* allow (but not implement) having different destinations for the wall and not just the standard output (choose by 
parameter)

To be clear, **you don't need to implement these scenarios**, but think about how your code could support at least some 
of them and what abstractions you would need.

### 💯 How we will review the challenge

We understand not everyone has the same available time to dedicate to a code challenge. We want to stress that we don't 
need a crazy implementation that covers every single scenario and edge case.

**What we will review with attention and value the most is, basically, your use of abstractions and patterns to provide a 
clean and open (to extension) solution following good practices.**

## 📒 Examples

These are some examples of the most simple solution.

`$> build 5 5`

![5 x 5 example](https://go.rviewer.io/wp-content/uploads/2022/06/5x5.png)

`$> build 10 7`

![5 x 5 example](https://go.rviewer.io/wp-content/uploads/2022/06/10x7.png)

`$> build "eight" [3]`

null


`$> build 12 -4`

null


`$> build 123 1024`

Naah, too much...here's my resignation.
