# RedirectHTTPS
Redirect http request to https for website hosted in IIS

Auto redirect http request to https after install SSL for a website hosted in IIS.
To begin:

* Clone this project to your server (or just coppy web.config to a folder, let's say "redirect" . You choose)
* Change web.config file content:  "https://www.yourWhatEverDomain" to your domain name or IP public.
* Disable port 80 in binding of target website on IIS.
* Create a website call "redirect" in IIS have physic path = path to "redirect" folder, binding to port 80
* Start new redirect you just create and done.

Your website now should redirect automaticaly to https when user request from http.
