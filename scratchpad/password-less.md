# Password-less Web Apps
For web applications, we have a nice secure(-ish) local container now in all greenfield browsers. So to oversimplify, a basic no-password strategy is literally:

1. First use _is_ registration. Store a unique token for this account + device + browser in an encrypted cookie or localstorage.  
2. allow user from device & browser #1 to use a capability URL to add another device/brower. make this capability URL expire (upon first use, or similar, depending on UX desired).  
3. upon visiting URL from #2, repeat step #1 for new device/browser.voila, you now have a password-less, device-authed system.

(cf. [my related thread on twitter](https://twitter.com/mrf1337/status/1354095045343924224?s=20))
<!--stackedit_data:
eyJoaXN0b3J5IjpbNjQ4NjMwNjcyXX0=
-->