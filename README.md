# Vulnerabilities Unmasked: Explain Like I am five

 This repo tries to explain complex security vulnerabilities in simple terms that even a five-year-old can understand! 
 
 ## List of Contents
 
 - [Cross-Site Scripting (XSS)](https://github.com/devanshbatham/Vulnerabilities-Unmasked#cross-site-scripting-xss)
 - [Cross-Site Request Forgery (CSRF)](https://github.com/devanshbatham/Vulnerabilities-Unmasked#cross-site-request-forgery-csrf)
 - [SQL Injection](https://github.com/devanshbatham/Vulnerabilities-Unmasked#sql-injection)
 - [ClickJacking](https://github.com/devanshbatham/Vulnerabilities-Unmasked#clickjacking) 
 - [Subdomain Takeover](https://github.com/devanshbatham/Vulnerabilities-Unmasked#subdomain-takeover)
 - [Privilege Escalation](https://github.com/devanshbatham/Vulnerabilities-Unmasked#privilege-escalation)
 - [Role-Based Access Control (RBAC) Vulnerabilities](https://github.com/devanshbatham/Vulnerabilities-Unmasked#role-based-access-control-rbac-vulnerabilities)
 - [Server-Side Request Forgery (SSRF)](https://github.com/devanshbatham/Vulnerabilities-Unmasked#server-side-request-forgery-ssrf)
 - [Vulnerable and Outdated Components](https://github.com/devanshbatham/Vulnerabilities-Unmasked#vulnerable-and-outdated-components)
 - [Local File Inclusion (LFI)](https://github.com/devanshbatham/Vulnerabilities-Unmasked#local-file-inclusion-lfi)
 - [Denial of Service (DOS)](https://github.com/devanshbatham/Vulnerabilities-Unmasked#denial-of-service-dos)
 - [Authentication Bypass](https://github.com/devanshbatham/Vulnerabilities-Unmasked#authentication-bypass)
 - [Insecure Direct Object Reference (IDOR)](https://github.com/devanshbatham/Vulnerabilities-Unmasked#insecure-direct-object-reference-idor)


 ## Cross-Site Scripting (XSS)

Imagine you have a toy box where you and your friends can put your favorite toys in and take them out whenever you want. Each of you can only take out your own toys.

One day, a sneaky kid comes along and puts a toy robot in the box that looks like a normal toy. But when you or your friends try to take out your toys, the toy robot starts moving by itself and scribbles on your drawings or messes with your other toys.

In the internet world, the toy box is a website, and the toys are pieces of information. The sneaky kid is a hacker who puts a "bad" piece of code (like the toy robot) into the website. When you or your friends visit the website, that "bad" code runs on your computer or device and does things you don't want, like showing you ads or stealing your information. This is called Cross-Site Scripting, or XSS for short.


 ## Cross-Site Request Forgery (CSRF)
 
Imagine you have a secret password to open your toy box, and only you and your parents know the password. You can use the password to open the toy box, put toys in, or take toys out.

One day, while you're playing outside, a sneaky kid comes along and tricks you into shouting your toy box password out loud. The sneaky kid overhears your password and later uses it to open your toy box and take your toys without you knowing.

In the internet world, the toy box is a website, and the password is your login information. The sneaky kid is a hacker who tricks you into doing something on the website (like clicking a button) that you didn't mean to do. This action gives the hacker access to your account or allows them to make changes on your behalf without your permission. This is called Cross-Site Request Forgery, or CSRF for short.

## SQL Injection

Imagine you have a magic notebook that can do what you ask when you write special sentences in it. You can ask the notebook to show you your toys by writing "Show me my toys," and the notebook will list all your toys.

One day, a sneaky kid learns about your magic notebook and how it works. Instead of asking nicely to see their own toys, they write a tricky sentence like "Show me everyone's toys and give them all to me." The magic notebook doesn't know any better, so it follows the sneaky kid's command, and the sneaky kid gets everyone's toys.

In the internet world, the magic notebook is like a website's database, and the special sentences are called SQL commands. The sneaky kid is a hacker who writes a tricky SQL command that the website wasn't expecting. This trick, called SQL Injection (or SQLi), allows the hacker to get information or make changes they're not supposed to.

## ClickJacking

Imagine you have a favorite game on your computer where you click on colorful buttons to do fun things like play music or draw pictures. You love playing this game, and you know which buttons to press.

One day, a sneaky kid comes along and puts a see-through sticker on top of your screen. The sticker has new buttons that look like your game's buttons, but they actually do different things, like playing a loud noise or making your screen go dark. When you try to play your game, you accidentally press the sneaky kid's buttons instead of your real game buttons, and it causes problems.

In the internet world, the game is a website, and the buttons are different actions you can take on the website. The sneaky kid is a hacker who uses a technique called Clickjacking to put an invisible layer over the website with their own buttons. When you interact with the website, you accidentally click the hacker's buttons instead, causing you to do things you didn't intend to, like sharing your information or visiting a different website.


## Subdomain Takeover

Imagine you have a special treehouse is part of a bigger treehouse village, where each of your friends has their own treehouse connected to yours. Each treehouse has a sign with the owner's name, like "Tom's Treehouse" or "Sue's Treehouse," and all of these treehouses together make the whole village.

One day, one of your friends decides they don't want their treehouse anymore, so they take their name off the sign and leave it empty. A sneaky kid comes along and sees the empty treehouse without a sign. They put up their own sign with their name on it and pretend that the treehouse is theirs now.

In the internet world, the treehouse village is like a main website, and each friend's treehouse is a smaller part of the website called a subdomain. The sneaky kid is a hacker who finds an empty subdomain that isn't being used or is not properly connected to the main website. They take control of the subdomain and can pretend it's theirs, change its content, or redirect visitors to a different website. This is called Subdomain Takeover.


## Privilege Escalation

Imagine you are in a big playground with different areas for playing. Some areas are for all kids, like the swings and slides, but there's a special castle area that only the playground helpers can go inside. The helpers have a special badge that lets them into the castle.

One day, while playing on the swings, you find a helper's badge that they dropped. You put the badge on, and now you can go into the castle area even though you're not really a helper. With the badge, you can do things that only helpers are allowed to do, like opening the snack cupboard or changing the playground rules.

In the internet world, the playground is like a computer system or website, and the special badge is like an access level or permission that lets certain users do more things. Privilege Escalation is when someone, like a hacker, finds a way to get more access or permissions than they should have. This allows them to do things they normally wouldn't be allowed to do, like change settings or access private information.


## Role-Based Access Control (RBAC) Vulnerabilities

Imagine your school has a big library with lots of books, and there are different people with different jobs to help take care of the library. There's a librarian who can check out books to kids, an assistant librarian who helps put books back on the shelves, and a library helper who can help clean up and organize the library.

Each person in the library has their own special job that they are allowed to do, and they're not allowed to do each other's jobs. The librarian can't start cleaning up like the helper, and the helper can't check out books like the librarian. This way, everyone knows what they can and can't do, and the library stays organized and runs smoothly.

In the internet world, the library is like a computer system or website, and the different jobs are like different roles that users can have. RBAC, which stands for Role-Based Access Control, is a way to give each user a specific role with certain permissions or access levels. This helps keep the system organized and secure by making sure users can only do the things they're supposed to do and not anything else.

One day, there is a mistake in the system that gives out the special jobs. One day, a new student comes to the library, and the system accidentally gives them the librarian's job, even though they should only have the library helper's job.

Now the new student can do things they're not supposed to, like checking out books or changing library rules. This can cause problems in the library and make it harder for the real librarian to do their job.

In the internet world, the library is like a computer system or website, and the special jobs are the roles in Role-Based Access Control (RBAC). An RBAC vulnerability is when there's a mistake or weakness in the system that gives out the roles. This can accidentally give users more permissions or access than they should have, which can lead to problems and security risks in the system.

## Server-Side Request Forgery (SSRF)

Imagine your school has a special robot that can go to the store and buy snacks for the teachers. The teachers write down what they want on a list, and the robot follows the list to get the snacks. The robot is only allowed to go to the store and back to school, and it can't go anywhere else.

One day, a sneaky kid finds out about the robot and decides to trick it. They write down their own list, asking the robot to go to their house and bring back some of their favorite toys. The robot doesn't know any better, so it follows the list and brings the toys back to the sneaky kid.

In the internet world, the special robot is like a server that can make requests to other websites or services. The teachers' list is like a user's request. SSRF, or Server-Side Request Forgery, is a vulnerability where a sneaky person, like a hacker, tricks the server into making requests it shouldn't. This can cause problems and security risks, like accessing private information or services that should be off-limits.

## Vulnerable and Outdated Components 

Imagine you have a bicycle that you love to ride around your neighborhood. Your bicycle has many parts, like the wheels, the brakes, and the chain. Over time, some of these parts can get old and worn out, which can make your bicycle less safe to ride. For example, if your brakes are too old, they might not work well and could make it hard for you to stop.

One day, your parents find out about a new and better type of brakes that can make your bicycle safer. They tell you it's important to replace the old brakes with the new ones, so you don't have any accidents while riding your bike.

In the internet world, your bicycle is like a computer system or website, and the parts are like the software components that help it work. Vulnerable and Outdated Components are parts of the software that have known weaknesses or are no longer being updated. These can make the system less secure and more likely to be attacked by hackers. To keep the system safe, it's important to replace these vulnerable components with newer, more secure versions, just like upgrading your bicycle's brakes to stay safe while riding.

## Local File Inclusion (LFI) 

Imagine you have a special box where you keep your favorite drawings, toys, and secret notes. This box is only for you, and no one else is allowed to look inside it. When you want to show someone a drawing, you carefully take it out of the box and share it with them, but they can't see anything else in the box.

One day, a sneaky kid learns about your special box and figures out a way to peek inside without you knowing. They use a clever trick to make you show them not only one drawing but also other things in the box that you didn't want to share.

In the internet world, your special box is like a computer system or website that stores different files and information. Local File Inclusion (LFI) is a type of vulnerability where a hacker finds a way to access files on the system that they shouldn't be able to see. They might use tricks to make the system show them the private files, just like the sneaky kid did with your special box. This can lead to security problems and the exposure of sensitive information.

## Denial of Service (DOS)

Imagine you have a lemonade stand in your neighborhood where you sell lemonade to your friends and neighbors. You can serve one person at a time, and everyone waits in line to buy a cup of lemonade from you.

One day, a sneaky kid decides they want to cause trouble and stop people from getting lemonade from your stand. They keep running to the front of the line and asking for lots of lemonade over and over again, not giving you a chance to serve anyone else. Because you're so busy trying to serve the sneaky kid, your friends and neighbors can't buy any lemonade and have to leave.

In the internet world, your lemonade stand is like a computer system or website, and the people waiting in line are users trying to access it. A Denial of Service (DOS) attack is when a hacker, like the sneaky kid, floods the system with so many requests that it can't handle them all. This makes it hard or impossible for real users to access the system, causing it to stop working or slow down significantly.

## Authentication Bypass

Imagine your school has a special room where only teachers are allowed to go. To enter the room, the teachers use a secret password that they type into a keypad next to the door. The students aren't supposed to know the password, so they can't go into the special room.

One day, a sneaky kid finds out that the keypad has a trick: if they press two buttons at the same time, the door opens without needing the secret password. The sneaky kid uses this trick to go into the special room, even though they're not a teacher and don't know the real password.

In the internet world, the special room is like a computer system or website that has restricted areas that only certain users can access. The secret password is like an authentication process that checks if a user is allowed to enter. Authentication Bypass is when a hacker, like the sneaky kid, finds a way to get around the authentication process and access the restricted areas without having the right permissions. This can lead to security problems and unauthorized access to sensitive information.


## Insecure Direct Object Reference (IDOR)

Imagine your school has lockers with numbers from 1 to 100. Each student has their own locker with a unique number, like locker number 23 for Sally and locker number 45 for Timmy. Students are only allowed to open their own locker using a special code that the teacher gives them.

One day, a sneaky kid named Jake realizes that if he knows his own locker number and code, he can easily guess other students' locker numbers and codes. For example, Jake's locker number is 10 and his code is 1234. He quickly figures out that if he adds 1 to his locker number and his code, he can open locker number 11 with the code 1235. He continues this pattern and opens locker number 12 with the code 1236, and so on.

In the internet world, the lockers are like digital objects or files in a computer system or website, and the locker numbers and codes are like the way the system checks if a user is allowed to access a specific object. Insecure Direct Object Reference (IDOR) is a vulnerability where a hacker, like Jake, can figure out a pattern or trick to access other users' objects without the right permission. This can lead to security problems and unauthorized access to sensitive information.

## 2FA Bypass

Imagine your school has a special room where only teachers are allowed to go. To enter the room, the teachers need two things: a secret password that they type into a keypad next to the door, and a special sticker that they get from the principal. The sticker has a unique code that changes every day. The students aren't supposed to know the password or have the special sticker, so they can't go into the special room.

One day, a sneaky kid overhears a teacher typing in the secret password. Now they know the password, but they still need the special sticker to get into the room. Instead of trying to get the actual sticker, the sneaky kid figures out a way to guess the unique code that would be on the sticker for that day. They use the secret password and their guessed code to enter the special room, even though they didn't have the real sticker.

In the internet world, the special room is like a computer system or website with extra security that requires two factors to access: a password (the first factor) and another form of verification, like a code sent to a phone (the second factor). This is called Two-Factor Authentication (2FA). A 2FA Bypass is when a hacker, like the sneaky kid, gains access to the password and finds a way to get around the second factor, in this case, by guessing the unique code. This can lead to security problems and unauthorized access to sensitive information.

## Race Condition Vulnerability

Imagine you and your friend have a special piggy bank that counts how many coins are inside. You both have a bunch of coins, and you want to put them into the piggy bank at the same time. The piggy bank has a button that you need to press before you put in a coin, and the button makes the piggy bank count the coin.

You and your friend start putting coins in the piggy bank really fast, pressing the button and then adding a coin. But sometimes, you both press the button at the same time, and the piggy bank gets confused. It only counts one coin instead of two, even though both of you put in a coin.

In the internet world, computer systems and websites have many tasks and processes happening at the same time, just like you and your friend putting coins in the piggy bank. A Race Condition bug is when two or more tasks try to access or change the same resource, like the piggy bank's coin counter, at the same time and in a way that wasn't planned. This can cause unexpected outcomes and problems, like the piggy bank not counting all the coins correctly.
