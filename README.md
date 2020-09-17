# Django on Azure

The web application used as an example in my writing of the article on **Serverless Python on Azure: Django hosted on Azure App Service**

## Tech
Written in Python3 and Django 3.1.1.

## Setup

* First, clone the repository:

```sh
git clone https://github.com/django_azure/core.git
cd django_azure
```

* Create a virtual environment to install dependencies in and activate it:


```sh
mkvirtualenv <envname>
source <envname>/bin/activate
```

* Install requirements in the virtual environment created:

```sh
pip install -r requirements.txt
```

* Run database migrations with this command

```sh
python3 manage.py migrate
```

* Run server to ensure everything is working properly.

```sh
python3 manage.py runserver
```

## Article Introduction

Over time, one of the most tiresome and non-rewarding tasks to some developers I know is the setup, maintenance and scaling of servers. Something often goes wrong.

Don't get me wrong, some developers like [me](https://paulonteri.com/) enjoy that process. 
However, it doesn't scale well and the repetition of tasks can get tiring. 

Doing all of this on your own can take some time:
* Operating system maintenance
* Capacity Provisioning - increase or reduce servers(or capacity) to handle different traffic
* Availability and fault tolerance
* Load balancing
* Networking

It's not a wonder that many companies like **Netflix, Uber, CodePen,** etc are using Serverless technology.

This article will cover the basics of deploying a basic Django(Python) application to Azure App Service, a serverless offering by Microsoft Azure. This will allow you to stop stressing or even **stop thinking about servers** in your development lifecycle.

What we'll cover:
* What is Serverless anyway? 👀
* Azure App Service
* Django Application setup
    1. Setting up a basic Django application
    2. Pushing the code to GitHub
* Deploying to Azure App Service
    1. Provisioning the target Azure App Service
    2. Deploy to App Service from GitHub
    3. Your App is now Deployed! 😎
* What Next?

Prerequisites:
* Basic web development understanding.
* Experience with git and GitHub. [Here's a simple guide](https://blog.usejournal.com/how-to-contribute-to-open-source-software-with-git-github-2b3be6e36c82?gi=3b86c4b3e2f7).
* Basic Python and Django experience. (If you'll follow the exact steps under the app setup)
* An Azure Account. (If you'll deploy)

...

---

### About me
I ❤️ anything around Software Development.

I currently work as a Frontend Dev at a company called Inuua Tujenge, working with React, React Native and Django (Python & JavaScript) almost daily.

Check out my most recent project - a [**Remote Code Execution Engine**](https://runcode.paulonteri.com/) like the ones on HackerRank and Leetcode.
It currently supports Python, JavaScript, Java, Go, C#, etc.

Feel free to [connect with me](https://paulonteri.com/). 👌

Thanks for your valuable time.


