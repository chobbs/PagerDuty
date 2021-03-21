# PagerDuty HTML Runbook Preview Files
Hosting for Runbook HTML files.

If you try to open raw version of any HTML, CSS or JS file in a web browser directly from GitHub, all you will see is a source code. GitHub forces them to use the "text/plain" content-type, so they cannot be interpreted. This script overrides it by using a CORS proxy.

Usage
In order to use it, just prepend this fragment to the URL of any HTML file: https://htmlpreview.github.io/? e.g.:

https://htmlpreview.github.io/?https://github.com/chobbs/PagerDuty/blob/main/Rb1.html
https://htmlpreview.github.io/?https://github.com/chobbs/PagerDuty/blob/main/Rb2.html

What it does is: load HTML using CORS proxy, then process all links, frames, scripts and styles, and load each of them using CORS proxy, so they can be evaluated by the browser.
