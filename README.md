# Pen Testing Live Targets

Time spent: 8 hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:

* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each color is vulnerable to only 2 of the 6 possible exploits. First discover which color has the specific vulnerability, then write a short description of how to exploit it, and finally demonstrate it using screenshots compiled into a GIF.

## Blue

Vulnerability #1: Insecure Direct Object Reference

Description: 
1) Under the "Find a Salesperson" section, upon clicking a name, we can see "https://35.184.88.145/blue/public/salesperson.php?id=1" as the URL
2) We use brute force to change the "id= " part of the URL
3) When trying using "...id=11" (i.e. "https://35.184.88.145/blue/public/salesperson.php?id=11"), we find that the RED site has an IDOR vulnerability
4) We are able to view a salesperson: "Lazy Lazyman(FIRED FOR STEALING)"

<img src="Unit_8_IDOR.gif">


## Green

Vulnerability #1: __________________

Description:

<img src="green-vuln1.gif">


## Red

Vulnerability #1: __________________

Description:

<img src="red-vuln1.gif">


## Notes

Describe any challenges encountered while doing the work

