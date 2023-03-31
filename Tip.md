- *One way*
> Take one bug type ad try to do as much as mastery on it. `Go deeper.` Go to the basics. 
> Distinguish between what can be automated and what can be not. Don't waste time on `what can be not automated.`
> Try to take technical as well as non technical bugs so you can trained yourself in both way. 

- *Another way*
> Be a "Hactivity Hunter"
> Take a disclosed fixed bug from Hactivity/CrowdStream and try to bypass the fixes.
> This will save your time to find out the vulnerable point of application, you don't need to find weakness, you need to find how to bypass the fixes. 
> This will again give you some kind of boost and help you to pass `Analysis Paralysis` phase.


- *One more way*
> A way to easy learning is to `follow hacker`. Follow one hacker and his methodology, in `steal like an artist` way. Just read his approach and articles and then turn to other hacker for the same. In the end, you will have your own methodology. 

- Some major points that should be focus on when do recon:
```
1. Try to get original IP. Use SecurityTrails or hakoriginfinder type tools. You may need ASN for domain.
2. If very big scope, do horizonal recon too. This will also help to understand the infrastructure and will trained you to deal with large program. 
3. Try to get all IPs. Get all subdomains and then get IPs.
4. Try to get all JS files. Then find secrets.
5. Try to get all subdomains to do FUZZ.
6. Try to URLs with parameter to try for XSS, SQLI or CMD injection.
7. Try to get URLs (as much as possible) to try Nuclei scan.
8. Use Gau-Exposed to gather multiple results.
9. Try to get all login pages. Try to bypass if interesting internal page - Authentication bypass.
```
 
- Make an user account and play, if for normal user. This is most important because here you need to do manual testing and you will get the chance to find IDOR, Business logic, Injection, File upload, Rate limit and much more. Without it, there is a very few chance to get a bug.
```
1. After registration, look for session related bugs.
2. After registration, go to setting/personal information page and look for business logic bugs and filter bypasses.
3. Notedown API endpoints when performing any operation, try to check API bugs.
4. Look for 2FA/OTP set, try to exploit them.
5. Make multiple account to findout IDOR related bugs.
6. Rate limit can be found in any submit button or in place where user perform any operation.
7. If you find any place where you can add URLs, try to exploit SSRF.
8. Look for profile pic or file upload functionality and try file upload exploitation.
9. For Blind XSS, look for file submission or feedback kind of pages. Look for reflective and Stored XSS too. All is possible.
10. SQL and Blind SQL is also possible to do if one try in input filed or submit operations.
```

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
