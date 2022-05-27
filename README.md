## WebCommand 
There is a polular package "WebTerminal" it is excellent in most situations.   
Except:   
- running system commands in your operating shell is not so easy    
- as it communicates to the IRIS host over HTTP and WSS it consumes 2 connections   
  With only 5 connectins in the community license (and teh "GraCE Period of CSP")   
  you can hit the limits rater fast: 2 Webterminal + 1 SMp and you are done    
- WebCommand is a pure CSP page consuming just 1 single connection    
- WebComamnd allows multiple ObjetScript command lines running in sequence    
- With **$** or **!** your command goes to Operating System as with default terminal    
- It is no full terminal emulation but a slim helper for debugging     
- And it is an excellent place to apply ["one-liners"](https://community.intersystems.com/post/one-liners-useful-objectscript-commands-one-line-long)    

## Prerequisites
Make sure you have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and [Docker desktop](https://www.docker.com/products/docker-desktop) installed.

## Installation 
Clone/git pull the repo into any local directory
```
git https://github.com/rcemper/Dataset-OEX-reviews.git
```
Run the IRIS container with your project: 
```
docker-compose up -d --build
```
## How to Test it

```
docker-compose exec iris iris session iris
```

**[or use Online Demo](https://dataset-oex-reviews.demo.community.intersystems.com/csp/sys/%25CSP.Portal.Home.zen) :**

### Example 1 

 ![](https://raw.githubusercontent.com/rcemper/IRIS-fast-ECP-setup/master/CodeQuality.JPG)

[Demo Server SMP](https://webcommand.demo.community.intersystems.com/csp/sys/UtilHome.csp)   
[Demo Server WebTerminal](https://webcommand.demo.community.intersystems.com/terminal/)    
        
**Code Quality**   
<img width="85%" src="
https://user-images.githubusercontent.com/31236645/147383045-964967ea-a7ba-4357-9012-1930c58b1806.png
">
