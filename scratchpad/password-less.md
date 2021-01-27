# Password-less Web Apps
For web applications, we have a nice secure(-ish) local container now in all greenfield browsers. A basic no-password strategy looks something like:

1. First use _is_ registration. Store a unique token for this account + device + browser trio, encrypted in a cookie or localstorage.  
2. In the app's account settings, provide an "Add a Device/Browser to This Account" [capability URL](https://www.w3.org/TR/capability-urls/), which folks may copy/email/text to themselves. **For security: Generate this capability URL on-demand, and make it expire immediately upon use.**
3. Upon visiting the capability URL from step #2, via any browser on any device, all registered devices/browsers are notified, and asked to confirm the new device/browser. The capability URL should expire immediately, whether or not confirmation is successful.
4. Upon confirmation from an registered device/browser, the new device + browser is added to the account, and step #1 is repeated for that new browser.

Voila, you now have a password-less, device-authed system. Implementation details such as notifications (browser? email? other?) are left to the reader. This is a gross oversimplification of what Signal, Keybase, WhatsApp, and others are already doing.

Want to see a smart implementation of password-less auth in a web app? Check out the work my friends @dyoder & @freeformflo have done over at http://dashkite.com.
DashKite: Be Yourself.
You're more than data for an algorithm. You're more than ad inventory. You deserve to feel safe and welcome. You deserve to have your privacy respected. You deserve to feel free to **be yourself.**...
dashkite.com
11:02 AM · Jan 26, 2021·Twitter for Android
Michael Fleet
@mrf1337
·
Jan 26
Replying to 
@mrf1337
They're also exploring how social media might be used to help solve  social problems like disinformation & extremism, instead of exacerbating them.
And how we repair it
@dyoder
·
22h
Replying to 
@mrf1337
 and 
@freeformflo
We're not *presently* using this specific technique (we'll be reintroducing it though). However, we are using capability-based authorization, which is arguably even cooler. 
Slightly smiling face
dashkite/cobalt
Sane Web Capabilities. Contribute to dashkite/cobalt development by creating an account on GitHub.
github.com


(cf. [my related thread on twitter](https://twitter.com/mrf1337/status/1354095045343924224?s=20))
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTk4MTg1MTA1MV19
-->