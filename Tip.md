Secret:
```
1. Read the reports; Hackerone as wll as Medium reports.
2. Replicate the reports, on the same target, follow the same steps; like a researcher.
3. Practice. Take any target. Practice on real targets.
4. 80% manual testing, 20% Automation.
5. Follow steps like a AI Bot. 
```


> Take one bug type ad try to do as much as mastery on it. `Go deeper.` Go to the basics. 
> Distinguish between what can be automated and what can be not. Don't waste time on `what can be not automated.`
> Try to take technical as well as non technical bugs so you can trained yourself in both way. 

- Some major points that should be focus on:
- Try to get original IP. Use SecurityTrails or hakoriginfinder type tools. You may need ASN for domain.
- Try to get all IPs. Get all subdomains and then get IPs.
- Try to get all JS files. Then find secrets.
- Try to get all subdomains to do FUZZ.
- Try to URLs with parameter to try for XSS, SQLI or CMD injection.
- Try to get URLs (as much as possible) to try Nuclei scan.
- Try to get all login pages. Try to bypass if interesting internal page.
- Make an user account and play, if for normal user. This is most important because here you need to do manual testing and you will get the chance to find IDOR, Business logic, Injection, File upload, Rate limit and much more. Without it, there is a very few chance to get a bug.

