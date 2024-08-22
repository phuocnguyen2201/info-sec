# info-sec
# h0 Hello, web!
a. Publish a web page. Show that you can make headings (h1 #, h2 ##...), paragraphs (p, empty line), links (a http://example.com) and code style (code or pre, four spaces at start of line). Markdown recommended.

# h1 Threat modeling
* The question **"What can go wrong"** repeatedly all over again through many articles, even in the podcast. It is really an important question in security scene, threat could be in any kind of **form, method**. Moreover, It's like a reminder to think and act like differently each time.
* After each of threat we been throught, we need to learn a lesson from it. Then we'll have principles for it, mainly help us with fast approach to root cause and tackle it as fast as we can, if we ever encouter it again.
* It is alway good to have a cheat sheet, it like a emergency book. Its help you to remind what step/ method to use in specific scenario. (If anyone watched Sully, the scene when the plane loose both engines and co-pilot have to quickly seek guidance in the book)

## Security hygiene
* When access restrict area, you should have a credential like identity card. You don't give/ borrow from someone else.
* Don't public any credential to online network.
* Don't click unverify URL/ Link.
* Change pw frequently.
* Don't store "hard" password with note or any application that do not apply any security method.

## Make-belief boogie-man
* Company H is an It consultant and outsoucing. Its threat modeling would be their employee's human error (leak client's information, contract, documentation ...)
* Their daily work will be, discuss business with client, analysis, define taskes and implementation.

1. What are we working on?
* Our assets: Cusomter's Personal Data, Contract, Documentation, Value of the contract, other vendor.
* Security: The office is cover with blur window. Secured network with requirement from customer.
* Cusomter is king: Employees do daily task, Manager keep close with Client. Output is deliver based on right date as promised.


2. What could go wrong?
* Spoofing: an Dev accidently upload API Key to github, and scanned by hacker.
* Tampering: the hacker create ton of virtual machine on cloud with stolen API Key, and start mining cryptocurrencies.
* Repudiation: the hacker turn off the alert for Pricing, and no one notice.
* Information Disclosure: they start extract any sensitive information on storage.
* Denial of Service: They dont do this because it will stop their VM.
* Elevation of Privileges: create new account with easily mistaken like admin, root for back-up.

3. What are we going to do about it?
* Don't share sensitive information with someone who not into project.
* Early - Training about security is needed for newbie.
* Change the working process, there must be well-review when upload thing to online.

4. Did we do a good enough job?
* Need review more careful, retrospective one time a month.
