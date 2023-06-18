# Vulnerabilities Unmasked: Explain Like I am five

 This repo tries to explain complex security vulnerabilities in simple terms that even a five-year-old can understand! 
 
 ## List of Contents
 
 
 
 ## XSS

Imagine you have a toy box where you and your friends can put your favorite toys in and take them out whenever you want. Each of you can only take out your own toys.

One day, a sneaky kid comes along and puts a toy robot in the box that looks like a normal toy. But when you or your friends try to take out your toys, the toy robot starts moving by itself and scribbles on your drawings or messes with your other toys.

In the internet world, the toy box is a website, and the toys are pieces of information. The sneaky kid is a hacker who puts a "bad" piece of code (like the toy robot) into the website. When you or your friends visit the website, that "bad" code runs on your computer or device and does things you don't want, like showing you ads or stealing your information. This is called Cross-Site Scripting, or XSS for short.


 ## CSRF
 
Imagine you have a secret password to open your toy box, and only you and your parents know the password. You can use the password to open the toy box, put toys in, or take toys out.

One day, while you're playing outside, a sneaky kid comes along and tricks you into shouting your toy box password out loud. The sneaky kid overhears your password and later uses it to open your toy box and take your toys without you knowing.

In the internet world, the toy box is a website, and the password is your login information. The sneaky kid is a hacker who tricks you into doing something on the website (like clicking a button) that you didn't mean to do. This action gives the hacker access to your account or allows them to make changes on your behalf without your permission. This is called Cross-Site Request Forgery, or CSRF for short.

## SQLi

Imagine you have a magic notebook that can do what you ask when you write special sentences in it. You can ask the notebook to show you your toys by writing "Show me my toys," and the notebook will list all your toys.

One day, a sneaky kid learns about your magic notebook and how it works. Instead of asking nicely to see their own toys, they write a tricky sentence like "Show me everyone's toys and give them all to me." The magic notebook doesn't know any better, so it follows the sneaky kid's command, and the sneaky kid gets everyone's toys.

In the internet world, the magic notebook is like a website's database, and the special sentences are called SQL commands. The sneaky kid is a hacker who writes a tricky SQL command that the website wasn't expecting. This trick, called SQL Injection (or SQLi), allows the hacker to get information or make changes they're not supposed to.

## ClickJacking

Imagine you have a favorite game on your computer where you click on colorful buttons to do fun things like play music or draw pictures. You love playing this game, and you know which buttons to press.

One day, a sneaky kid comes along and puts a see-through sticker on top of your screen. The sticker has new buttons that look like your game's buttons, but they actually do different things, like playing a loud noise or making your screen go dark. When you try to play your game, you accidentally press the sneaky kid's buttons instead of your real game buttons, and it causes problems.

In the internet world, the game is a website, and the buttons are different actions you can take on the website. The sneaky kid is a hacker who uses a technique called Clickjacking to put an invisible layer over the website with their own buttons. When you interact with the website, you accidentally click the hacker's buttons instead, causing you to do things you didn't intend to, like sharing your information or visiting a different website.



