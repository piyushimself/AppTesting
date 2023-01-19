To hunt target.com, 

1st step is to understand the app. So try to find following:

- [ ]  Start to understand first what type of service it is.
- [ ]  How many type of users?
- [ ]  Who will be a user? Is it B2B, B2C or some kind of sharing platform like social media?
- [ ]  What will be the important data for them?
- [ ]  Scope and functionality to find bug.
- [ ]  How interested the team is to solve the security issues?

2nd step is to find out technical information about application like:

- [ ]  What server they are using?
- [ ]  What web framework they are using?
- [ ]  Is there any old updated component that they are using?
- [ ]  Can we see session related data in inspect element, how it is looking?
- [ ]  See the source code, what it is look like?

Next, in 3rd step, we should try to map the application.

- [ ]  Where we can input data?
- [ ]  Can we take output of processed input data?
- [ ]  What type of functionality is common in all the pages?
- [ ]  Which functionality is in only one page?
- [ ]  Can we insert <>’”- char?
- [ ]  What is there in response for a request?
- [ ]  How application behave when we create 404,401 etc request?
- [ ]  What type of payloads and wordlist will be good to interact with application?

Then, in 4rt step, we are going to follow checklist to attack all kind of attacks. This is most important step where expertise is important. Not all the attacks are important to master. What attacks we should try is depend upon the previous steps i.e. nature of the application and what we have got after mapping.

- [ ]  https://www.notion.so/spinthehack/Checklist-2-After-Recon-Deep-Inside-6a2d8c280a28498d8ad7c38568603b2d
- [ ]  https://www.notion.so/spinthehack/Checklist-2-After-Recon-Deep-Inside-6a2d8c280a28498d8ad7c38568603b2d
- [ ]  https://pentestbook.six2dez.com/
- [ ]  https://cheatsheet.haax.fr/
- [ ]  https://book.hacktricks.xyz/welcome/readme

5th and last step is actually very important. It is to note down everything that you feel important.
- If anything unique, note down.
- If anything is important that you know you can compare with other user, note down. 
- Note down the URLs too, as sometime we miss whare we found something that is needed in future.
- Make mind map of application and place the functions and type of possible attack there. 
- Note down credentials and session data for that particular user.
