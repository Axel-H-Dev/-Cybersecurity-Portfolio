# Lab: Basic SSRF against the local server

## Objective

Exploit a Server-Side Request Forgery (SSRF) vulnerability to access an
internal admin panel hosted on `localhost` and delete the user `carlos`.

## Skills Practiced

-   Server-Side Request Forgery (SSRF)
-   Burp Suite (Proxy & Repeater)
-   HTTP request manipulation
-   Internal service access

## Methodology

1.  Intercepted the stock check request with Burp Suite.
2.  Modified the `stockApi` parameter to target the internal admin
    endpoint.
3.  Confirmed access to the internal administration interface.
4.  Changed the request to the delete endpoint for the target user.
5.  Verified successful exploitation.

## Tools

-   Burp Suite Community Edition
-   Web Browser
-   PortSwigger Web Security Academy

## Result

**Lab solved successfully.**

------------------------------------------------------------------------

**Author:** Axel Hernandez
