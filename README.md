# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

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

Vulnerability #1: SQL Injection (SQLi)

Description: The salesperson info page is vulnerable to SQL injection. As an example, you can put the following in the url. This will cause the site to wait for 7 seconds before processing the request.

    ?id=5' or sleep(7)=0--'
   
<img src="blue-vuln1.gif">

Vulnerability #2: Session Hijacking/Fixation

Description: I opened two instances of the login page in two browsers. I logged in one of the browser and copied its session id. I changed the session id for another browser with the session id I copied. This allowed the other browser to be logged in without using the login credentials.

<img src="blue-vuln2.gif">

## Green

Vulnerability #1: Cross-Site Scripting (XSS)

Description: Open up the contact form and put the malicious code inside the feedback box. Here, an alert box pops up when an admin/user opens up the feedback page.

    <script>alert('Anjal found the XSS!')</script>

<img src="green-vuln1.gif">

Vulnerability #2: __________________

Description:

<img src="green-vuln2.gif">


## Red

Vulnerability #1: __________________

Description:

<img src="red-vuln1.gif">

Vulnerability #2: __________________

Description:

<img src="red-vuln2.gif">


## Notes

Describe any challenges encountered while doing the work
