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


## Subdomain Takeover

Imagine you have a special treehouse is part of a bigger treehouse village, where each of your friends has their own treehouse connected to yours. Each treehouse has a sign with the owner's name, like "Tom's Treehouse" or "Sue's Treehouse," and all of these treehouses together make the whole village.

One day, one of your friends decides they don't want their treehouse anymore, so they take their name off the sign and leave it empty. A sneaky kid comes along and sees the empty treehouse without a sign. They put up their own sign with their name on it and pretend that the treehouse is theirs now.

In the internet world, the treehouse village is like a main website, and each friend's treehouse is a smaller part of the website called a subdomain. The sneaky kid is a hacker who finds an empty subdomain that isn't being used or is not properly connected to the main website. They take control of the subdomain and can pretend it's theirs, change its content, or redirect visitors to a different website. This is called Subdomain Takeover.


## Privilege Escalation

Imagine you are in a big playground with different areas for playing. Some areas are for all kids, like the swings and slides, but there's a special castle area that only the playground helpers can go inside. The helpers have a special badge that lets them into the castle.

One day, while playing on the swings, you find a helper's badge that they dropped. You put the badge on, and now you can go into the castle area even though you're not really a helper. With the badge, you can do things that only helpers are allowed to do, like opening the snack cupboard or changing the playground rules.

In the internet world, the playground is like a computer system or website, and the special badge is like an access level or permission that lets certain users do more things. Privilege Escalation is when someone, like a hacker, finds a way to get more access or permissions than they should have. This allows them to do things they normally wouldn't be allowed to do, like change settings or access private information.


## RBAC Issues

Imagine your school has a big library with lots of books, and there are different people with different jobs to help take care of the library. There's a librarian who can check out books to kids, an assistant librarian who helps put books back on the shelves, and a library helper who can help clean up and organize the library.

Each person in the library has their own special job that they are allowed to do, and they're not allowed to do each other's jobs. The librarian can't start cleaning up like the helper, and the helper can't check out books like the librarian. This way, everyone knows what they can and can't do, and the library stays organized and runs smoothly.

In the internet world, the library is like a computer system or website, and the different jobs are like different roles that users can have. RBAC, which stands for Role-Based Access Control, is a way to give each user a specific role with certain permissions or access levels. This helps keep the system organized and secure by making sure users can only do the things they're supposed to do and not anything else.

One day, there is a mistake in the system that gives out the special jobs. One day, a new student comes to the library, and the system accidentally gives them the librarian's job, even though they should only have the library helper's job.

Now the new student can do things they're not supposed to, like checking out books or changing library rules. This can cause problems in the library and make it harder for the real librarian to do their job.

In the internet world, the library is like a computer system or website, and the special jobs are the roles in Role-Based Access Control (RBAC). An RBAC vulnerability is when there's a mistake or weakness in the system that gives out the roles. This can accidentally give users more permissions or access than they should have, which can lead to problems and security risks in the system.

## SSRF

Imagine your school has a special robot that can go to the store and buy snacks for the teachers. The teachers write down what they want on a list, and the robot follows the list to get the snacks. The robot is only allowed to go to the store and back to school, and it can't go anywhere else.

One day, a sneaky kid finds out about the robot and decides to trick it. They write down their own list, asking the robot to go to their house and bring back some of their favorite toys. The robot doesn't know any better, so it follows the list and brings the toys back to the sneaky kid.

In the internet world, the special robot is like a server that can make requests to other websites or services. The teachers' list is like a user's request. SSRF, or Server-Side Request Forgery, is a vulnerability where a sneaky person, like a hacker, tricks the server into making requests it shouldn't. This can cause problems and security risks, like accessing private information or services that should be off-limits.
