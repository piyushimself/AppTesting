
> Take one bug type ad try to do as much as mastery on it. `Go deeper.` Go to the basics. 
> Distinguish between what can be automated and what can be not. Don't waste time on `what can be not automated.`
> Try to take technical as well as non technical bugs so you can trained yourself in both way. 

- One more way
> A way to easy learning is to `follow hacker`. Follow one hacker and his methodology, `steal like an artist` way. Just read his approach and articles and then turn to other hacker for the same. In the end, you will have your own methodology. 

- Some major points that should be focus on:
- Try to get original IP. Use SecurityTrails or hakoriginfinder type tools. You may need ASN for domain.
- If very big scope, do horizonal recon too. This will also help to understand the infrastructure and will trained you to deal with large program. 
- Try to get all IPs. Get all subdomains and then get IPs.
- Try to get all JS files. Then find secrets.
- Try to get all subdomains to do FUZZ.
- Try to URLs with parameter to try for XSS, SQLI or CMD injection.
- Try to get URLs (as much as possible) to try Nuclei scan.
- Try to get all login pages. Try to bypass if interesting internal page.
- Make an user account and play, if for normal user. This is most important because here you need to do manual testing and you will get the chance to find IDOR, Business logic, Injection, File upload, Rate limit and much more. Without it, there is a very few chance to get a bug.

> Try to learn/update yourself with hunting. It is very important to do both simultaniously. `Make 2-3 hr to learn/update and 2-3 hr to hunt`. Do automation, run code, read write ups, open browser and look for web resources at the time of learning. Take a target and apply learning at the time of hunting. `For hunting, if not getting anything right, use the secret`. Both time, taking notes is very important. But, take notes at the time of learning to remember and make process easy but take notes at the time of hunting to make hunting easy. `Don't mix anything`. For best results and avoid burn out, make plan before start to learn or hunt. This will give your mind a definite task. 

### Secret:
```
1. Read the reports; Hackerone as wll as Medium reports.
2. Replicate the reports, on the same target, follow the same steps; like a researcher.
3. Practice. Take any target. Practice on real targets.
4. 80% manual testing, 20% Automation.
5. Follow steps like a AI Bot. 
```

### Attack Points.
```
1. Proxies - HTTP Request smuggling, Server side inclusion, Cache poisoning
2. User Input -> Reflected Values - Injections, SSRF
3. Search Functionalities - SQL, File inclusion, ReDOS
4. Forms, WebSockets and PostMsgs - CSRF
5. HTTP Headers - Cookie hacking, Clickjacking, CSP
6. Bypasses - 2FA, Rate limit, Race condition, Captcha, Login, Payment process, Registration
7. Structured objects / Specific functionalities - Email header, XML, JWT
8. Files - File upload, Formula injection, server side xss
9. External Identity Management - OAuth to takeover
10. Other Helpful Vulnerabilities - IDOR, Takeover, Parameter Pollution, 
```
