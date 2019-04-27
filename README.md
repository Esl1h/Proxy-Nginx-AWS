# Proxy to AWS services

[![N|nginx](https://www.nginx.com/wp-content/uploads/2019/01/logo.svg)](https://nginx.org)

 - Problem:
For various reasons, some clients in my app can not use it because their networks have IP address blocking (and can not release domains / fqdn, the release is done only by IP) and how the app has its infrastructure within AWS , using services such as S3, cloudfront, lambda, API Gateway ... It enters into a very large range of addresses and CDN, making it impossible to release the IPs.

Solution:
Proxy (with Public IP / EIP) using Ngnix to do the redirect.
