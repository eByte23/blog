Title: Deploying with CodeDeploy and CloudFormation
Published: 1/10/2018
Tags: ["Developer","AWS","CodeDeploy","CI","Cloud"]
Author: Elijah Bate
---

### The Problem
I had just updated our api from .netcore2 > .netcore 2.1 this cause the ami image that it was running on to fail to run our api.
This caused a deployment loop where it continuously created and toredown 10's of ec2 instances
[Screenshot here(show teardowns)]

The issue was i needed to create the new image
[Screenshot here(Show where image is)]

then change the parameter in codedeploy


