# ReCaptcha V3 Solver

Fastest, cheapest and highest quality ReCaptcha V3 solver.

Please ignore this app if you don't need it, or if you are satisfied with the results of the services, or the results of another similar apps.

![](./tests-screen.jpg)

## Features

### Solutions Quality

Score 0.9 for 99% of tokens (captcha solutions).
Guaranteed if conditions are met:

-   Good mobile or redirected proxies of any country, except RU.
-   Change of IP is obligatory after each solution
-   Repeated use of IP no more than 1 time in 2 hours

Hosting or any Russian ip's can't guarantee high solutions score.

### Speed of solutions

Less than a second per solution, starting from the second solved captcha.

Guaranteed under the conditions:

-   Proxies are fast enough.
    Sometimes solution time can reach 25 seconds.

### Low traffic consumption

On the average 25 kb per one solution of captchas.

### Change of IP by link

It can be useful for working with proxies having rotation by the link.

### Emulation of API of popular services

Supported:

- RuCaptcha
- 2Captcha
- Anticaptcha

If you write queries from scratch, follow instructions from [here](https://anti-captcha.com/apidoc) or [here](https://2captcha.com/2captcha-api), then change the host of the link to your own.
For example: the application runs locally (127.0.0.1) on port 5555, in this case change the link like this:

**For RuCaptcha/2Captcha API**:

- http://rucaptcha.com/in.php --> http://127.0.0.1:5555/in.php
- http://rucaptcha.com/res.php --> http://127.0.0.1:5555/res.php

**For Anticaptcha API**:

- https://api.anti-captcha.com/createTask --> http://127.0.0.1:5555/createTask
- https://api.anti-captcha.com/getTaskResult --> http://127.0.0.1:5555/getTaskResult

If you use ready-made solutions and there is no possibility to change the link, you can add a rule to the hosts file.

To do this:

- Run the application on port 80
- Open as administrator the file c:{windows\system32\drivers\etc\hosts
- Add the following lines to the very end
- `127.0.0.1 rucaptcha.com`
- `127.0.0.1 anti-captcha.com`
- Save this file

### Support for Enterprise version of captcha

## Other

Free for a limited time.

`There is no technical support for setup or anything else.`

The application is delivered "as is" and if you are not happy with the use - ignore app.
