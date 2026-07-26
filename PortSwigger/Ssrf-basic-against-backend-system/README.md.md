# Lab: Basic SSRF against another back-end system

## Objective

Identify an internal back-end host through SSRF, access its
administration interface, and delete the user `carlos`.

## Skills Practiced

-   SSRF against internal networks
-   Burp Suite Intruder
-   Repeater
-   Internal network enumeration
-   HTTP analysis

## Methodology

1.  Intercepted the stock request.
2.  Used Intruder to enumerate internal IP addresses.
3.  Identified the host exposing the admin interface.
4.  Sent the successful request to Repeater.
5.  Modified the request to call the delete endpoint for `carlos`.
6.  Confirmed successful exploitation.

## Tools

-   Burp Suite Community Edition
-   PortSwigger Web Security Academy

## Result

**Lab solved successfully.**

------------------------------------------------------------------------

**Author:** Axel Hernandez
