Title: Using a Custom Domain from CloudFlare with API Gateway
Published: 1/10/2018
Tags: ["Developer","AWS","CloudFlare"]
Author: Elijah Bate
---

I found it really hard to get this working.

But the answer was simple when I read alot of blogs

1. Ensure all your domain and certificate are adding in to region where your services is, sometimes this still doesn't work so you have to add it too `us-east-1`
2. Make sure you select edge not region when assigning a custom domain in api gateway
3. Assign your domain to the "target" domain shown after you create the custom domain **NOTE** it may take upto 40 minutes to start working (Most of the time)
4. The target domain its self will not work until you assign the cname