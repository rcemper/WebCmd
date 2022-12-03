## WebCommand 
There is a popular package "WebTerminal". It is excellent in most situations.   
Except:   
- running system commands in your operating shell is not so easy    
- as it communicates to the IRIS host over HTTP and WSS it consumes 2 connections   
  With only 5 connections in the community license (and the "Grace Period of CSP")   
  you can hit the limits rater fast: 2 Webterminals + 1 SMP and you are done    
- WebCommand is a pure CSP page consuming just 1 single connection    
- WebCommand allows multiple ObjectScript command lines running in sequence    
- With **$** or **!** your command goes to Operating System same as with default terminal    
- It is no full terminal emulation but a slim helper for debugging     
- And it is an excellent place to apply ["One Liners"](https://community.intersystems.com/post/one-liners-useful-objectscript-commands-one-line-long)    

## Prerequisites
Make sure you have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and [Docker desktop](https://www.docker.com/products/docker-desktop) installed.

## Installation 
Clone/git pull the repo into any local directory
```
git https://github.com/isc-at/WebCommand.git
```
Run the IRIS container with your project: 
```
docker-compose up -d --build
```
## How to Test it

http://localhost:42773/csp/user/webcmd.csp   

**[or use Online Demo](https://webcommand.demo.community.intersystems.com/csp/user/webcmd.csp) :**

### Examples

- Just a simple loop in ObjectScript   
<img width="70%" src="https://community.intersystems.com/sites/default/files/inline/images/images/image(3922).png">    

- Directory listing inside container
 <img width="70%" src="https://community.intersystems.com/sites/default/files/inline/images/images/image(3923).png">   
 
 - File Dump
 <img width="70%" src="https://community.intersystems.com/sites/default/files/inline/images/images/image(3924).png">   


[Article on DC](https://community.intersystems.com/post/webcommand)    
