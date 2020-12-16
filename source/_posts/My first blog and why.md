---
title: From zero to 1, how to create your own blog
tags: blog
index_img: /img/blog2.jpg
---
![](/img/blog2.jpg)
## Background
### why I want strart writing blog
Creating a blog was an idea I had in few weeks ago. I tried many times before and after but all ended in failure. Recently, my idea of creating a blog has become stronger and stronger. Accidently I found out that I can create my own blog by using GitHub. And there is what you see now.

Before I was a person who relied heavily on social media. Every time I turn on the phone, the first thing I do is watch video,  post and check what others have done aimlessly. At that moment I don’t feel my-self. In this era of “information explosion”, I found slowly that I became unable to think independently. So I gradually stay away from various social media such as Facebook, Weibo, QQ, etc. The main reason why I stay away from them is very simple because they give me innutritious information all the time.

I hope that in this blog I can quietly be my-self and write down my true feelings. Here I hope I can think freely, without considering other people's feelings. This is also my original intention of creating this blog. In addition, I also want to record every moment of this young man, after all you are still worth remembering in this rushed world. Whenever this young man wants to look back, at least there are stories that belong to him, and some of his whimsical thoughts.

  2020-12-14

  Z.H.



## How to create a blog using GitHub and Hexo
In this page I gonna introduce how to use Github and Hexo to build your own static website or blog. Let's go it will be fun and fun :D.
## GitHub
### Short intro about github
The first thing you need is GitHub.


## Hexo
### What is Hexo and why you need it?
Basically Hexo is a blog framework that allows you to quickly build a blog. In my case I chose Hexo because it is fast, concise and efficient. Hexo is written by Node.js and it also supports Markdown and many other packages. Hence you actually don't need that much programming och computer knowledge like HTML、css、JavaScript etc. The only thing you should learn or feel familiar with is Markdown. Of course if you want your blog to look prefekt and beautiful that is strong recommend that you master the basics programming language like HTML.
### Install Hexo
This installation is based on operating system Linux distro Ubuntu. The first thing you have to do is install Node.js. You can do it by using following command in terminal:

cURL:
``` bash
$ curl https://raw.github.com/creationix/nvm/v0.33.11/install.sh | sh
```
Wget:
``` bash
$ wget -qO- https://raw.github.com/creationix/nvm/v0.33.11/install.sh | sh
```
After the installation is complete, restart the terminal and execute the following commands to install Node.js.
``` bash
$ nvm install stable
```
When it is finish then you can use npm to install Hexo.
``` bash
$ npm install -g hexo-cli
```
### Configure Hexo
When Hexo is finished installed, then you are prepared to build your own static website/blogg.
First create a empty folder:
``` bash
mkdir <your_blog_name>
```
then install Hexo into the folder
```bash
hexo init <your_blog_name>
```
Yeee, your website is created!!! Easy, right? Let move on!!!
____
Attention: you maybe have to execute this command before you execute hexo.
```bash
source ~/.nvm/nvm.sh
```
____
Next thing you have to do is configure your website. After Hexo is install at your folder, you will se a document with name ```_config.yml```. I know it looks complex but don’t give up. We will go through this document step by step and show how you configure your website. (I will be back)

### Deploy Hexo
Above I showed you how to install hexo and create a website. Now you may want to publish it. To do it you have to deploy to GitHub first and install the deployment plugin. To install he deployment plugin you can do with following command:
```bash
$ npm install hexo-deployer-git --save
$ npm install hexo-server --save
```
If you never used GitHub and git before then you must configure git. Like:
```bash
$ git config --global user.name "Your_user_name"
$ git config --global user.email "Your_email@example.com"
```

Then you go back till```_config.yml``` and you will find ```deploy``` below the document. Then filli
```bash
deploy:
  type: git
  repo: <repository url>
  branch: master (main or master it depends)
  message:<if you want>
```
When you are finish, then in the root directory of the local Hexo site, execute the following commands to deploy to GitHub:
```bash
source ~/.nvm/nvm.sh (maybe)
$ hexo clean && hexo d -g
```
Tadda, looks how easy it is. Now you publish your website successfully. There are few more things that I want to show you, first you may notice your website does not look beautiful. Hence the next step is how to change the theme so your blog looks more elegant. Second is about the domain name of your website. A great domain name makes more people remember your site and also gives your more confidence.
### Install theme
I my case I use theme fluid.
