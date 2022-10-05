We've prepared you a repository with a kata from [rviewer.io](https://go.rviewer.io/dev-build-a-wall/) in order to show your skills.

Clone this repository, you can commit your changes in the main branch. Once you completed the task you must create a [git patch](https://www.git-tower.com/learn/git/faq/create-and-apply-patch/) and send it over to us via email.

The aim of this Challenge is to create the strongest wall of all time! You will have to combine bricks, in a proper way, to avoid instability.

# HOW IT WORKS
This is a CLI application that receives 2 arguments and represent the created wall in ASCII.

To do so, your CLI command have to receive the following parameters:

- Number of rows: The number of rows of bricks the wall has to have
- Number of bricks: The number of bricks you have to use on each row to represent the wall

# HOW TO REPRESENT YOUR WALL

To represent your one-and-only creation you have to use the following elements:

✔️ ■■: A full brick (2 of ■). The bigger brick for the wall

✔️ ■: Half a brick. The smallest unit

✔️ |: Mortar. The cement between each brick on the same row


# HOW TO BUILD A STRONG WALL
Any builder knows that, if you just put a brick over another, your wall is going to fall down as you turn your
back!

To build a strong wall you have to follow these considerations:

There has to be a mortar (|) every brick (half or full) on the same row
Bricks cannot be aligned vertically with the bricks of the row above or below it, to provide more stability

# Examples

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
