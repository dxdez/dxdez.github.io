---
layout: page
title: Resources
permalink: /resources/
---
## **Table of Contents**
- [Assets and Tools](#assets-and-tools)
  - [General Tools and Resources](#general-tools-and-resources)
  - [Docker, NGINX and Deployment Resources](#docker-nginx-and-deployment-resources)
  - [Audio Resources](#audio-resources)
  - [CSS Frameworks](#css-frameworks)
- [Linux](#linux)
- [JavaScript](#javascript)
- [C/C++](#cc)
  - [Network programming](#network-programming)
  - [OpenGL](#opengl)
  - [Compilation and Debugging](#compilation-and-debugging)
  - [C](#c)
  - [C++](#c-1)
- [Go](#go)
- [Python](#python)
  - [Project Ideas and Resources](#project-ideas-and-resources)
  - [Web Scraping](#web-scraping)
  - [Web Applications](#web-applications)
  - [Bots](#bots)
  - [Data Science](#data-science)
  - [Machine Learning](#machine-learning)
  - [OpenCV](#opencv)
  - [Deep Learning](#deep-learning)
  - [Miscellaneous](#miscellaneous)
- [Rust](#rust)

## **Assets and Tools**

#### **General Tools and Resources**
- [Markdown Guide](https://www.markdownguide.org/basic-syntax/) - The Markdown elements outlined in the original design document.
- [SVG Pro](https://www.svgrepo.com/ "SVG Pro") - Search, explore and edit the best-fitting free icons or vectors for your projects using a wide variety vector library. 
- [Cloud Converter](https://cloudconvert.com/ "Cloud Converter") - A resource that allows various file formats to be converted into a different format (i.e. png to ico)
- [Extends Class Developer Tools](https://extendsclass.com/ "Extends Class Developer Tools") - A collection of tools for developers to help with formatting and organizing code.
- [Favicons](https://favicon.io/emoji-favicons/ "Favicons") - Free emoji icons that can be used in a project.
- [Nerd Fonts](https://www.nerdfonts.com/font-downloads "Nerd Fonts") - Fonts put together for use in an IDE or terminal.
- [Porkbun](https://porkbun.com/ "Porkbun") - A domain name registrar with lower prices on domain registrations and renewals.
- [KeyBR](https://www.keybr.com/account "KeyBR") - A resource for improveing typing speed on the keyboard.
- [Geeks for Geeks](https://www.geeksforgeeks.org/ "Geeks for Geeks") - A resource for develoeprs which include various articles, guides on data structures and video tutorials on various subjects.

#### **Docker, NGINX and Deployment Resources**
- [Docker Documentation](https://hub.docker.com/ "Docker Documentation") - Basic documentation for using Docker
- [Docker with React/Vue and Vite](https://dev.to/ysmnikhil/how-to-build-with-react-or-vue-with-vite-and-docker-1a3l "Docker with React/Vue and Vite") - An article that provides steps on using the Vite runtime with a Docker container for a React or Vue project
- [Geeks for Geeks Docker Resource](https://www.geeksforgeeks.org/containerization-using-docker/?ref=lbp "Geeks for Geeks Docker Resource") - Resources provided by Geeks for Geeks on using Docker
- [Docker Exec](https://docs.docker.com/reference/cli/docker/container/exec/ "Docker Exec") - A common command; this documentation shows the use of the exec function and running shell commands within Docker
- [Dockerize a React/Vite Project](https://www.webdevolution.com/blog/how-to-use-docker-with-react-and-vite/ "Dockerize a React/Vite Project") - This guide provides an overview on creating a basic docker container for a react application
- [NGINX Documentation](https://docs.nginx.com/nginx/ "NGINX Documentation") - The documentation for NGINX; includes setting up web servers and proxies
- [Serving Multiple Websites with a Single Nginx Server](https://www.youtube.com/watch?v=HWrhSpN4ar0 "Serving Multiple Websites with a Single Nginx Server") - A basic guide on using NGINX proxies to host multiple domains on a single server
- [How to Host Multiple Docker Containers on a Single Server with Nginx Reverse Proxy](https://www.youtube.com/watch?v=spbkCihFpQ8 "How to Host Multiple Docker Containers on a Single Server with Nginx Reverse Proxy?") - Hosting several docker containers through an NGINX Reverse Proxy
- [Production Ready VPS with Go, Docker and Traefik](https://www.youtube.com/watch?v=F-9KWQByeU0 "Production Ready VPS with Go, Docker and Traefik") - Setting up a production ready VPS using tools such as Docker, Traefik and covering essentials such as hardened SSH and SSL


#### **Audio Resources**
- [sfxr](https://drpetter.se/projectsfxr.html "sfxr") - Legacy software that can be used to generate some new sounds
- [ChipTone](https://sfbgames.itch.io/chiptone "ChipTone") - Online resource for generating simple wave files for sound effects
- [FamiTracker](http://www.famitracker.com/links.php "FamiTracker") - An additional audio resources for creating audio files
- [Programming Benchmarks](https://programming-language-benchmarks.vercel.app "Programming Benchmarks") - Online resource for comparing various programming benchmarks
- [LMMS](https://lmms.io/ "LMMS") - Official site for LMMS, an open source tool for creating audio tracks
- [LMMS Repo](https://github.com/LMMS/lmms "LMMS Repo") - The Github repository for LMMS

#### **CSS Frameworks**
- [PicoCSS](https://picocss.com/) - Minimal CSS Framework for Semantic HTML
- [BeerCSS](https://www.beercss.com/) - Build material design interfaces in record time

## **Linux**
- [HowToForge](https://www.howtoforge.com/ "HowToForge") - A helpful resource on using various programs and utilities within linux both on the server and desktop
- [Updating Fedora with DNF and YUM](https://www.fosslinux.com/93984/how-to-update-fedora-by-gui-and-command-line-ways.htm "Updating Fedora with DNF and YUM") - A simple article on covering the basics with the default package manager in Fedora Linux.  This guide covers the basics in running dnf and yum commands.
- [Creating the 'll' alias](https://forums.linuxmint.com/viewtopic.php?t=109177 "Creating the 'll' alias") - This forum posts covers the basics in creating a custom terminal alias for certain commands. By default, some distributions do not use the 'll' shortcut which is shortened from 'ls -l'. This posts covers creating one. 
- [SSH Server Setup in Arch Linux](https://linuxhint.com/arch_linux_ssh_server/ "SSH Server Setup in Arch Linux") - This article will show you how to install, customize and optimize SSH server on Arch Linux. 
- [i3 Gaps Setup in Arch Linux](https://low-orbit.net/arch-linux-how-to-install-i3-gaps "i3 Gaps Setup in Arch Linux") - This article will cover the essential steps in creating an i3 setup within Arch Linux. The starting point of this guide assume a basic TTY setup within an Arch installation.
- [Unlock SU with Root password](https://superuser.com/questions/280048/root-password-is-not-working-for-su-in-terminal "Unlock SE with Root password") - If the SU key in terminal is not working, these steps will unlock the root user for SU command.
- [GREP Overview](https://www.howtoforge.com/tutorial/linux-grep-command/ "Grep Overview") - An overview of the GREP utility in linux which can be used to locate files and strings within a directory of files
- [Checking Directory Size, 3 Methods](https://www.redswitches.com/blog/check-the-size-of-a-directory-in-linux/#:~:text=The%20du%20command%20is%20used,in%20a%20human%2Dreadable%20format. "Checking Directory Size, 3 Methods") - This article shows 3 different ways for analyzing directory size
- [System Cleanup, Fedora/RHEL](https://developers.redhat.com/blog/2020/12/10/how-to-clean-up-the-fedora-root-folder# "System Cleanup, Fedora/RHEL") - This article provides some common solutions for cleaning up diskspace such as pruning non-used docker images, clearing unused kernels and querying large folders for bloat
- [Making Executable Files in Linux](https://gcore.com/learning/how-to-make-file-executable-in-linux/ "Making Executable Files in Linux") - This article provides guidance on executing files in Linux
- [LibreOffice Development]("https://www.libreoffice.org/community/developers/") - Resources on contributing to the LibreOffice project
- [Linux Handbook](https://linuxhandbook.com/ "Linux Handbook") - A helpful site with a variety of articles on maintaining a linux server and setting up a devops pipeline on linux

## **JavaScript**
- [You might not need jQuery](https://youmightnotneedjquery.com/)
- [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript?tab=readme-ov-file#standard-library)
 
## **C/C++**

#### **Network programming**
- Let's Code a TCP/IP Stack
  - [Part 1: Ethernet & ARP](http://www.saminiir.com/lets-code-tcp-ip-stack-1-ethernet-arp/)
  - [Part 2: IPv4 & ICMPv4](http://www.saminiir.com/lets-code-tcp-ip-stack-2-ipv4-icmpv4/)
  - [Part 3: TCP Basics & Handshake](http://www.saminiir.com/lets-code-tcp-ip-stack-3-tcp-handshake/)
  - [Part 4: TCP Data Flow & Socket API](http://www.saminiir.com/lets-code-tcp-ip-stack-4-tcp-data-flow-socket-api/)
  - [Part 5: TCP Retransmission](http://www.saminiir.com/lets-code-tcp-ip-stack-5-tcp-retransmission/)
- Programming Concurrent Servers
  - [Part 1 - Introduction](https://eli.thegreenplace.net/2017/concurrent-servers-part-1-introduction/)
  - [Part 2 - Threads](https://eli.thegreenplace.net/2017/concurrent-servers-part-2-threads/)
  - [Part 3 - Event-driven](https://eli.thegreenplace.net/2017/concurrent-servers-part-3-event-driven/)
  - [Part 4 - libuv](https://eli.thegreenplace.net/2017/concurrent-servers-part-4-libuv/)
  - [Part 5 - Redis case study](https://eli.thegreenplace.net/2017/concurrent-servers-part-5-redis-case-study/)
  - [Part 6 - Callbacks, Promises and async/await](https://eli.thegreenplace.net/2018/concurrent-servers-part-6-callbacks-promises-and-asyncawait/)

#### **OpenGL**
  - [Breakout](https://learnopengl.com/In-Practice/2D-Game/Breakout)
  - [Setting up](https://learnopengl.com/In-Practice/2D-Game/Setting-up)
  - [Rendering Sprites](https://learnopengl.com/In-Practice/2D-Game/Rendering-Sprites)
  - [Levels](https://learnopengl.com/In-Practice/2D-Game/Levels)
  - Collisions
    - [Ball](https://learnopengl.com/In-Practice/2D-Game/Collisions/Ball)
    - [Collision detection](https://learnopengl.com/In-Practice/2D-Game/Collisions/Collision-detection)
    - [Collision resolution](https://learnopengl.com/In-Practice/2D-Game/Collisions/Collision-resolution)
  - [Particles](https://learnopengl.com/In-Practice/2D-Game/Particles)
  - [Postprocessing](https://learnopengl.com/In-Practice/2D-Game/Postprocessing)
  - [Powerups](https://learnopengl.com/In-Practice/2D-Game/Powerups)
  - [Audio](https://learnopengl.com/In-Practice/2D-Game/Audio)
  - [Render text](https://learnopengl.com/In-Practice/2D-Game/Render-text)
  - [Final thoughts](https://learnopengl.com/In-Practice/2D-Game/Final-thoughts)

#### **Compilation and Debugging**
- Write a C compiler
  - [Part 1: Integers, Lexing and Code Generation](https://norasandler.com/2017/11/29/Write-a-Compiler.html)
  - [Part 2: Unary Operators](https://norasandler.com/2017/12/05/Write-a-Compiler-2.html)
  - [Part 3: Binary Operators](https://norasandler.com/2017/12/15/Write-a-Compiler-3.html)
  - [Part 4: Even More Binary Operators](https://norasandler.com/2017/12/28/Write-a-Compiler-4.html)
  - [Part 5: Local Variables](https://norasandler.com/2018/01/08/Write-a-Compiler-5.html)
  - [Part 6: Conditionals](https://norasandler.com/2018/02/25/Write-a-Compiler-6.html)
  - [Part 7: Compound Statements](https://norasandler.com/2018/03/14/Write-a-Compiler-7.html)
  - [Part 8: Loops](https://norasandler.com/2018/04/10/Write-a-Compiler-8.html)
  - [Part 9: Functions](https://norasandler.com/2018/06/27/Write-a-Compiler-9.html)
  - [Part 10: Global Variables](https://norasandler.com/2019/02/18/Write-a-Compiler-10.html)
- Writing a Linux Debugger
  - [Part 1: Setup](https://blog.tartanllama.xyz/writing-a-linux-debugger-setup/)
  - [Part 2: Breakpoints](https://blog.tartanllama.xyz/writing-a-linux-debugger-breakpoints/)
  - [Part 3: Registers and memory](https://blog.tartanllama.xyz/writing-a-linux-debugger-registers/)
  - [Part 4: Elves and dwarves](https://blog.tartanllama.xyz/writing-a-linux-debugger-elf-dwarf/)
  - [Part 5: Source and signals](https://blog.tartanllama.xyz/writing-a-linux-debugger-source-signal/)
  - [Part 6: Source-level stepping](https://blog.tartanllama.xyz/writing-a-linux-debugger-dwarf-step/)
  - [Part 7: Source-level breakpoints](https://blog.tartanllama.xyz/writing-a-linux-debugger-source-break/)
  - [Part 8: Stack unwinding](https://blog.tartanllama.xyz/writing-a-linux-debugger-unwinding/)
  - [Part 9: Handling variables](https://blog.tartanllama.xyz/writing-a-linux-debugger-variables/)
  - [Part 10: Advanced topics](https://blog.tartanllama.xyz/writing-a-linux-debugger-advanced-topics/)
- Let's write a compiler
  - [Part 1: Introduction, selecting a language, and doing some planning](https://briancallahan.net/blog/20210814.html)
  - [Part 2: A lexer](https://briancallahan.net/blog/20210815.html)
  - [Part 3: A parser](https://briancallahan.net/blog/20210816.html)
  - [Part 4: Testing](https://briancallahan.net/blog/20210817.html)
  - [Part 5: A code generator](https://briancallahan.net/blog/20210818.html)
  - [Part 6: Input and output](https://briancallahan.net/blog/20210819.html)
  - [Part 7: Arrays](https://briancallahan.net/blog/20210822.html)
  - [Part 8: Strings, forward references, and conclusion](https://briancallahan.net/blog/20210826.html)

#### **C**
- [Let's Build a Simple Database](https://cstack.github.io/dbtutorial/)
- [Linux containers in 500 lines of code](https://blog.lizzie.io/linux-containers-in-500-loc.html)
- [Write your Own Virtual Machine](https://justinmeiners.github.io/lc3-vm/)
- [Writing a Game Boy emulator, Cinoop](https://cturt.github.io/cinoop.html)
- [Beej's Guide to Network Programming](http://beej.us/guide/bgnet/)
- [Let's code a TCP/IP stack](http://www.saminiir.com/lets-code-tcp-ip-stack-1-ethernet-arp/)
- [Operating Systems: From 0 to 1](https://tuhdo.github.io/os01/)
- [The little book about OS development](https://littleosbook.github.io/)
- [Roll your own toy UNIX-clone OS](http://jamesmolloy.co.uk/tutorialhtml/)
- [Kernel 101 – Let’s write a Kernel](https://arjunsreedharan.org/post/82710718100/kernel-101-lets-write-a-kernel)
- [Kernel 201 – Let’s write a Kernel with keyboard and screen support](https://arjunsreedharan.org/post/99370248137/kernel-201-lets-write-a-kernel-with-keyboard)
- [Baby's First Garbage Collector](http://journal.stuffwithstuff.com/2013/12/08/babys-first-garbage-collector/)
- [Build Your Own Lisp: Learn C and build your own programming language in 1000 lines of code](http://www.buildyourownlisp.com/)
- [Writing a Simple Garbage Collector in C](http://maplant.com/gc.html)
- [C interpreter that interprets itself.](https://github.com/lotabout/write-a-C-interpreter)
- [A C & x86 version of the "Let's Build a Compiler" by Jack Crenshaw](https://github.com/lotabout/Let-s-build-a-compiler)
- [A journey explaining how to build a compiler from scratch](https://github.com/DoctorWkt/acwj)
- [A Regular Expression Matcher](https://www.cs.princeton.edu/courses/archive/spr09/cos333/beautiful.html)
- [Regular Expression Matching Can Be Simple And Fast](https://swtch.com/~rsc/regexp/regexp1.html)
- [Writing a UNIX Shell](https://indradhanush.github.io/blog/writing-a-unix-shell-part-1/)
- [Write a shell in C](https://danishpraka.sh/posts/write-a-shell/)
- [Build Your Own Text Editor](https://viewsourcecode.org/snaptoken/kilo/)
- [How to Write a Video Player in Less Than 1000 Lines](http://dranger.com/ffmpeg/ffmpeg.html)
- [Learn how to write a hash table in C](https://github.com/jamesroutley/write-a-hash-table)
- [The very basics of a terminal emulator](https://www.uninformativ.de/blog/postings/2018-02-24/0/POSTING-en.html)
- [Write a Shell in C](https://brennan.io/2015/01/16/write-a-shell-in-c/)
- [Write a System Call](https://brennan.io/2016/11/14/kernel-dev-ep3/)
- [Sol - An MQTT broker from scratch](https://codepr.github.io/posts/sol-mqtt-broker)
- [Write a Bootloader in C](http://3zanders.co.uk/2017/10/13/writing-a-bootloader/)

#### **C++**
- [Introduction to Ray Tracing: a Simple Method for Creating 3D Images](https://www.scratchapixel.com/lessons/3d-basic-rendering/introduction-to-ray-tracing/how-does-it-work)
- [How OpenGL works: software rendering in 500 lines of code](https://github.com/ssloy/tinyrenderer/wiki)
- [Raycasting engine of Wolfenstein 3D](http://lodev.org/cgtutor/raycasting.html)
- [Physically Based Rendering:From Theory To Implementation](http://www.pbr-book.org/)
- [Ray Tracing in One Weekend](https://raytracing.github.io/books/RayTracingInOneWeekend.html)
- [Rasterization: a Practical Implementation](https://www.scratchapixel.com/lessons/3d-basic-rendering/rasterization-practical-implementation/overview-rasterization-algorithm)
- [Build Your Own Redis from Scratch](https://build-your-own.org/redis)
- [Breakout](https://learnopengl.com/In-Practice/2D-Game/Breakout)
- [Beginning Game Programming v2.0](http://lazyfoo.net/tutorials/SDL/)
- [Space Invaders from Scratch](http://nicktasios.nl/posts/space-invaders-from-scratch-part-1.html)
- [Writing a Bootloader](http://3zanders.co.uk/2017/10/13/writing-a-bootloader/)
- [Game physics series by Allen Chou](http://allenchou.net/game-physics-series/)
- [How to Create a Custom Physics Engine](https://gamedevelopment.tutsplus.com/series/how-to-create-a-custom-physics-engine--gamedev-12715)
- [Designing a Simple Text Editor](http://www.fltk.org/doc-1.1/editor.html)

## **Go**
- [GO By Example](https://gobyexample.com/ "GO By Example") - A step by step guide in teaching the GO programming language. Simple examples are provided to help the end user develop with Go.
- [GO Tour](https://go.dev/tour "GO Tour") - A step by step guide on the basics of GO
- [Learn GO with Tests](https://quii.gitbook.io/learn-go-with-tests/ "Learn GO with Tests") - A tutorial series for building an application in GO with automated unit tests
- [Effective GO](https://go.dev/doc/effective_go "Effective GO") - This document gives tips for writing clear, idiomatic Go code. It augments the language specification, the Tour of Go, and How to Write Go Code, all of which you should read first. 
- [Build Your Own Database from Scratch: Persistence, Indexing, Concurrency](https://build-your-own.org/database/)
- [Build Your Own Redis from Scratch](https://www.build-redis-from-scratch.dev/)
- [Build a multilayer perceptron with Golang](https://made2591.github.io/posts/neuralnetwork)
- [How to build a simple artificial neural network with Go](https://sausheong.github.io/posts/how-to-build-a-simple-artificial-neural-network-with-go/)
- [Building a Neural Net from Scratch in Go](https://datadan.io/blog/neural-net-with-go)
- [How to build a regex engine from scratch](https://rhaeguard.github.io/posts/regex)
- [Build A Simple Terminal Emulator In 100 Lines of Golang](https://ishuah.com/2021/03/10/build-a-terminal-emulator-in-100-lines-of-go/)
- [Let's Create a Simple Load Balancer](https://kasvith.me/posts/lets-create-a-simple-lb-go/)
- [Building Go Web Applications and Microservices Using Gin](https://semaphoreci.com/community/tutorials/building-go-web-applications-and-microservices-using-gin)
- [How to Use Godog for Behavior-driven Development in Go](https://semaphoreci.com/community/tutorials/how-to-use-godog-for-behavior-driven-development-in-go)
- [Go WebAssembly Tutorial - Building a Calculator Tutorial](https://tutorialedge.net/golang/go-webassembly-tutorial/)

## **Python**
- [Automate the Boring Stuff](https://automatetheboringstuff.com/)
- [Invent with Python](https://inventwithpython.com/)
- [Python Formatter](https://extendsclass.com/python-formatter.html)

#### **Project Ideas and Resources**
- [A 3D Modeller](http://aosabook.org/en/500L/a-3d-modeller.html)
- [DBDB: Dog Bed Database](http://aosabook.org/en/500L/dbdb-dog-bed-database.html)
- [Write your own miniature Redis with Python](http://charlesleifer.com/blog/building-a-simple-redis-server-with-python/)
- [A workshop on Linux containers: Rebuild Docker from Scratch](https://github.com/Fewbytes/rubber-docker)
- [A proof-of-concept imitation of Docker, written in 100% Python](https://github.com/tonybaloney/mocker)
- [ugit: Learn Git Internals by Building Git Yourself](https://www.leshenko.net/p/ugit/)
- [Implement a Neural Network from Scratch](https://victorzhou.com/blog/intro-to-neural-networks/)
- [Optical Character Recognition (OCR)](http://aosabook.org/en/500L/optical-character-recognition-ocr.html)
- [Traffic signs classification with a convolutional network](https://navoshta.com/traffic-signs-classification/)
- [Generate Music using LSTM Neural Network in Keras](https://towardsdatascience.com/how-to-generate-music-using-a-lstm-neural-network-in-keras-68786834d4c5)
- [An Introduction to Convolutional Neural Networks](https://victorzhou.com/blog/intro-to-cnns-part-1/)
- [Build Your Own Regular Expression Engines: Backtracking, NFA, DFA](https://build-your-own.org/b2a/r0intro)
- [Building a search engine using Redis and redis-py](http://www.dr-josiah.com/2010/07/building-search-engine-using-redis-and.html)
- [Building a Vector Space Indexing Engine in Python](https://boyter.org/2010/08/build-vector-space-search-engine-python/)
- [Developing a License Plate Recognition System with Machine Learning in Python](https://medium.com/devcenter/developing-a-license-plate-recognition-system-with-machine-learning-in-python-787833569ccd)
- [Building a Facial Recognition Pipeline with Deep Learning in Tensorflow](https://hackernoon.com/building-a-facial-recognition-pipeline-with-deep-learning-in-tensorflow-66e7645015b8)
- [Browser Engineering](https://browser.engineering)
- [Building a basic HTTP Server from scratch in Python](http://joaoventura.net/blog/2017/python-webserver/)
- [Continuous Integration System](http://aosabook.org/en/500L/a-continuous-integration-system.html)

#### **Web Scraping**
- [Mining Twitter Data with Python](https://marcobonzanini.com/2015/03/02/mining-twitter-data-with-python-part-1/)
- [Scrape a Website with Scrapy and MongoDB](https://realpython.com/blog/python/web-scraping-with-scrapy-and-mongodb/)
- [How To Scrape With Python and Selenium WebDriver](http://www.byperth.com/2018/04/25/guide-web-scraping-101-what-you-need-to-know-and-how-to-scrape-with-python-selenium-webdriver/)
- [Which Movie Should I Watch using BeautifulSoup](https://medium.com/@nishantsahoo.in/which-movie-should-i-watch-5c83a3c0f5b1)

#### **Web Applications**
- [A Simple Web Server](http://aosabook.org/en/500L/a-simple-web-server.html)
- [Let’s Build A Web Server.](https://ruslanspivak.com/lsbaws-part1/)
- [Web application from scratch](https://defn.io/2018/02/25/web-app-from-scratch-01/)
- [Build a Microblog with Flask](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)
- [Create a Blog Web App In Django](https://tutorial.djangogirls.org/en/)
- [Choose Your Own Adventure Presentations](https://www.twilio.com/blog/2015/03/choose-your-own-adventures-presentations-wizard-mode-part-1-of-3.html)
- [Build a Todo List with Flask and RethinkDB](https://realpython.com/blog/python/rethink-flask-a-simple-todo-list-powered-by-flask-and-rethinkdb/)
- [Build a Todo List with Django and Test-Driven Development](http://www.obeythetestinggoat.com/)
- [Build a RESTful Microservice in Python](http://www.skybert.net/python/developing-a-restful-micro-service-in-python/)
- [Microservices with Docker, Flask, and React](https://testdriven.io/)
- [Build A Simple Web App With Flask](https://pythonspot.com/flask-web-app-with-python/)
- [Create A Django API in under 20 minutes](https://codeburst.io/create-a-django-api-in-under-20-minutes-2a082a60f6f3)
- Build a Community-driven delivery application with Django, Postgres and JavaScript
  - [Part 1](https://www.ashwinhariharan.tech/blog/thinking-of-building-a-contact-tracing-application-heres-what-you-can-do-instead/)
  - [Part 2](https://www.ashwinhariharan.tech/blog/thinking-of-building-a-contact-tracing-application-heres-what-you-can-do-instead-part-2/)
- Realtime Chat application with Vue, django-notifs, RabbitMQ and uWSGI
  - [Part 1](https://danidee10.github.io/2018/01/01/realtime-django-1.html)
  - [Part 2](https://danidee10.github.io/2018/01/03/realtime-django-2.html)
  - [Part 3](https://danidee10.github.io/2018/01/07/realtime-django-3.html)
  - [Part 4](https://danidee10.github.io/2018/01/10/realtime-django-4.html)
  - [Part 5](https://danidee10.github.io/2018/01/13/realtime-django-5.html)
  - [Part 6](https://danidee10.github.io/2018/03/12/realtime-django-6.html)

#### **Bots**
- [Build a Reddit Bot](http://pythonforengineers.com/build-a-reddit-bot-part-1/)
- [How to Make a Reddit Bot - YouTube](https://www.youtube.com/watch?v=krTUf7BpTc0) (video)
- [Build a Facebook Messenger Bot](https://blog.hartleybrody.com/fb-messenger-bot/)
- [Making a Reddit + Facebook Messenger Bot](https://pythontips.com/2017/04/13/making-a-reddit-facebook-messenger-bot/)
- How To Create a Telegram Bot Using Python
  - [Part 1](https://khashtamov.com/en/how-to-create-a-telegram-bot-using-python/)
  - [Part 2](https://khashtamov.com/en/how-to-deploy-telegram-bot-django/)
- [Create a Twitter Bot In Python](https://medium.freecodecamp.org/creating-a-twitter-bot-in-python-with-tweepy-ac524157a607)

#### **Data Science**
- Learn Python For Data Science by Doing Several Projects (video):
  - [Part 1: Introduction](https://www.youtube.com/watch?v=T5pRlIbr6gg)
  - [Part 2: Twitter Sentiment Analysis](https://www.youtube.com/watch?v=oOZdbCzHUA)
  - [Part 3: Recommendation Systems](https://www.youtube.com/watch?v=9gBC9R-msAk&list=PL2-dafEMk2A6QKz1mrk1uIGfHkC1zZ6UU&index=3)
  - [Part 4: Predicting Stock Prices](https://www.youtube.com/watch?v=SSu00IRRraY&index=4&list=PL2-dafEMk2A6QKz1mrk1uIGfHkC1zZ6UU)
  - [Part 5: Deep Dream in TensorFlow](https://www.youtube.com/watch?v=MrBzgvUNr4w&list=PL2-dafEMk2A6QKz1mrk1uIGfHkC1zZ6UU&index=5)
  - [Part 6: Genetic Algorithms](https://www.youtube.com/watch?v=dSofAXnnFrY&index=6&list=PL2-dafEMk2A6QKz1mrk1uIGfHkC1zZ6UU)

#### **Machine Learning**
- [Write Linear Regression From Scratch in Python](https://www.youtube.com/watch?v=uwwWVAgJBcM) (video)
- [Step-By-Step Machine Learning In Python](https://machinelearningmastery.com/machine-learning-in-python-step-by-step/)
- [Predict Quality Of Wine](https://medium.freecodecamp.org/using-machine-learning-to-predict-the-quality-of-wines-9e2e13d7480d)
- [Solving A Fruits Classification Problem](https://towardsdatascience.com/solving-a-simple-classification-problem-with-python-fruits-lovers-edition-d20ab6b071d2)
- [Learn Unsupervised Learning with Python](https://scikit-learn.org/stable/unsupervisedlearning.html)
- [Build Your Own Neural Net from Scratch in Python](https://towardsdatascience.com/how-to-build-your-own-neural-network-from-scratch-in-python-68998a08e4f6)
- [Linear Regression in Python without sklearn](https://medium.com/we-are-orb/linear-regression-in-python-without-scikit-learn-50aef4b8d122)
- [Multivariate Linear Regression without sklearn](https://medium.com/we-are-orb/multivariate-linear-regression-in-python-without-scikit-learn-7091b1d45905)
- [Music Recommender using KNN](https://towardsdatascience.com/how-to-build-a-simple-song-recommender-296fcbc8c85)
- Find Similar Quora Questions-
  - [Using BOW, TFIDF and Xgboost](https://towardsdatascience.com/finding-similar-quora-questions-with-bow-tfidf-and-random-forest-c54ad88d1370)
  - [Using Word2Vec and Xgboost](https://towardsdatascience.com/finding-similar-quora-questions-with-word2vec-and-xgboost-1a19ad272c0d)
- [Detecting Fake News with Python and Machine Learning](https://data-flair.training/blogs/advanced-python-project-detecting-fake-news/)
- [Learn ML Algorithms by coding: Decision Trees](https://lethalbrains.com/learn-ml-algorithms-by-coding-decision-trees-439ac503c9a4)
- [JSON Decoding Algorithm](https://github.com/cheery/json-algorithm)

#### **OpenCV**
- [Build A Document Scanner](https://www.pyimagesearch.com/2014/09/01/build-kick-ass-mobile-document-scanner-just-5-minutes/)
- [Build A Face Detector using OpenCV and Deep Learning](https://www.pyimagesearch.com/2018/02/26/face-detection-with-opencv-and-deep-learning/)
- [Build fastest custom object Detection system yusing YOLOv3(video playlist)](https://www.youtube.com/playlist?list=PLKHYJbyeQ1a0oGzgRXy-QwAN1tSV4XZxg)
- [Build a Face Recognition System using OpenCV, Python and Deep Learning](https://www.pyimagesearch.com/2018/06/18/face-recognition-with-opencv-python-and-deep-learning/)
- [Detect The Salient Features in an Image](https://www.pyimagesearch.com/2018/07/16/opencv-saliency-detection/)
- [Build A Barcode Scanner](https://www.pyimagesearch.com/2018/05/21/an-opencv-barcode-and-qr-code-scanner-with-zbar/)
- [Learn Face Clustering with Python](https://www.pyimagesearch.com/2018/07/09/face-clustering-with-python/)
- [Object Tracking with Camshift](https://www.pyimagesearch.com/wp-content/uploads/2014/11/opencvcrashcoursecamshift.pdf)
- [Semantic Segmentation with OpenCV and Deep Learning](https://www.pyimagesearch.com/2018/09/03/semantic-segmentation-with-opencv-and-deep-learning/)
- [Text Detection in Images and Videos](https://www.pyimagesearch.com/2018/08/20/opencv-text-detection-east-text-detector/)
- [People Counter using OpenCV](https://www.pyimagesearch.com/2018/08/13/opencv-people-counter/)
- [Tracking Multiple Objects with OpenCV](https://www.pyimagesearch.com/2018/08/06/tracking-multiple-objects-with-opencv/)
- [Neural Style Transfer with OpenCV](https://www.pyimagesearch.com/2018/08/27/neural-style-transfer-with-opencv/)
- [OpenCV OCR and Text Recognition](https://www.pyimagesearch.com/2018/09/17/opencv-ocr-and-text-recognition-with-tesseract/)
- [Text Skew Correction Tutorial](https://www.pyimagesearch.com/2017/02/20/text-skew-correction-opencv-python/)
- [Facial Landmark Detection Tutorial](https://www.pyimagesearch.com/2017/04/03/facial-landmarks-dlib-opencv-python/)
- [Object Detection using Mask-R-CNN](https://www.learnopencv.com/deep-learning-based-object-detection-and-instance-segmentation-using-mask-r-cnn-in-opencv-python-c/)
- [Automatic Target Detection Tutorial](https://www.pyimagesearch.com/2015/05/04/target-acquired-finding-targets-in-drone-and-quadcopter-video-streams-using-python-and-opencv/)
- [EigenFaces using OpenCV](https://www.learnopencv.com/eigenface-using-opencv-c-python/)
- [Faster(5-point) Facial Landmark Detection Tutorial](https://www.pyimagesearch.com/2018/04/02/faster-facial-landmark-detector-with-dlib/)
- [Hand Keypoint Detection](https://www.learnopencv.com/hand-keypoint-detection-using-deep-learning-and-opencv/)
- Dlib Correlation Object Tracking -
  - [Single Object Tracker](https://www.pyimagesearch.com/2018/10/22/object-tracking-with-dlib/)
  - [Mutiple Object Tracker](https://www.pyimagesearch.com/2018/10/29/multi-object-tracking-with-dlib/)
- [Image Stitching with OpenCV and Python](https://www.pyimagesearch.com/2018/12/17/image-stitching-with-opencv-and-python/)
- [Instance Segmentation with OpenCV](https://www.pyimagesearch.com/2018/11/26/instance-segmentation-with-opencv/)
- [Face mask detector](https://www.pyimagesearch.com/2020/05/04/covid-19-face-mask-detector-with-opencv-keras-tensorflow-and-deep-learning/)

#### **Deep Learning**
- [Using Convolutional Neural Nets to Detect Facial Keypoints](http://danielnouri.org/notes/2014/12/17/using-convolutional-neural-nets-to-detect-facial-keypoints-tutorial/)
- [Generate an Average Face using Python and OpenCV](https://www.learnopencv.com/average-face-opencv-c-python-tutorial/)
- [Break A Captcha System using CNNs](https://medium.com/@ageitgey/how-to-break-a-captcha-system-in-15-minutes-with-machine-learning-dbebb035a710)
- [Use pre-trained Inception model to provide image predictions](https://medium.com/google-cloud/keras-inception-v3-on-google-compute-engine-a54918b0058)
- [Create your first CNN](https://hackernoon.com/deep-learning-cnns-in-tensorflow-with-gpus-cba6efe0acc2)
- [Build A Facial Recognition Pipeline](https://hackernoon.com/building-a-facial-recognition-pipeline-with-deep-learning-in-tensorflow-66e7645015b8)
- [Build An Image Caption Generator](https://medium.freecodecamp.org/building-an-image-caption-generator-with-deep-learning-in-tensorflow-a142722e9b1f)
- [Make your Own Face Recognition System](https://medium.freecodecamp.org/making-your-own-face-recognition-system-29a8e728107c)
- [Train a Language Detection AI in 20 minutes](https://towardsdatascience.com/how-i-trained-a-language-detection-ai-in-20-minutes-with-a-97-accuracy-fdeca0fb7724)
- [Object Detection With Neural Networks](https://towardsdatascience.com/object-detection-with-neural-networks-a4e2c46b4491)
- Learn Twitter Sentiment Analysis -
  - [Part I - Data Cleaning](https://towardsdatascience.com/another-twitter-sentiment-analysis-bb5b01ebad90)
  - [Part II - EDA, Data Visualisation](https://towardsdatascience.com/another-twitter-sentiment-analysis-with-python-part-2-333514854913)
  - [Part III - Zipf's Law, Data Visualisation](https://towardsdatascience.com/another-twitter-sentiment-analysis-with-python-part-3-zipfs-law-data-visualisation-fc9eadda71e7)
  - [Part IV - Feature Extraction(count vectoriser)](https://towardsdatascience.com/another-twitter-sentiment-analysis-with-python-part-4-count-vectorizer-b3f4944e51b5)
  - [Part V - Feature Extraction(Tfidf vectoriser)](https://towardsdatascience.com/another-twitter-sentiment-analysis-with-python-part-5-50b4e87d9bdd)
  - [Part VI - Doc2Vec](https://towardsdatascience.com/another-twitter-sentiment-analysis-with-python-part-6-doc2vec-603f11832504)
  - [Part VII - Phrase Modeling + Doc2Vec](https://towardsdatascience.com/another-twitter-sentiment-analysis-with-python-part-7-phrase-modeling-doc2vec-592a8a996867)
  - [Part VIII - Dimensionality Reduction](https://towardsdatascience.com/another-twitter-sentiment-analysis-with-python-part-8-dimensionality-reduction-chi2-pca-c6d06fb3fcf3)
  - [Part IX - Neural Nets with Tfdif vectors](https://towardsdatascience.com/another-twitter-sentiment-analysis-with-python-part-9-neural-networks-with-tfidf-vectors-using-d0b4af6be6d7)
  - [Part X - Neural Nets with word2vec/doc2vec](https://towardsdatascience.com/another-twitter-sentiment-analysis-with-python-part-10-neural-network-with-a6441269aa3c)
  - [Part XI - CNN with Word2Vec](https://towardsdatascience.com/another-twitter-sentiment-analysis-with-python-part-11-cnn-word2vec-41f5e28eda74)
- [Use Transfer Learning for custom image classification](https://becominghuman.ai/transfer-learning-retraining-inception-v3-for-custom-image-classification-2820f653c557)
- [Learn to Code a simple Neural Network in 11 lines of Python](https://iamtrask.github.io/2015/07/12/basic-python-network/)
- [Build a Neural Network using Gradient Descent Approach](https://iamtrask.github.io/2015/07/27/python-network-part2/)
- [Train a Keras Model To Generate Colors](https://heartbeat.fritz.ai/how-to-train-a-keras-model-to-generate-colors-3bc79e54971b)
- [Get Started with Keras on a Custom Dataset](https://www.pyimagesearch.com/2018/09/10/keras-tutorial-how-to-get-started-with-keras-deep-learning-and-python/)
- [Use EigenFaces and FisherFaces on Faces94 dataset](https://nicholastsmith.wordpress.com/2016/02/18/eigenfaces-versus-fisherfaces-on-the-faces94-database-with-scikit-learn/)
- [Kaggle MNIST Digit Recognizer Tutorial](https://medium.com/@lvarruda/how-to-get-top-2-position-on-kaggles-mnist-digit-recognizer-48185d80a2d4)
- [Fashion MNIST tutorial with tf.keras](https://medium.com/tensorflow/hello-deep-learning-fashion-mnist-with-keras-50fcff8cd74a)
- [CNN using Keras to automatically classify root health](https://www.pyimagesearch.com/2018/10/15/deep-learning-hydroponics-and-medical-marijuana/)
- [Keras vs Tensorflow](https://www.pyimagesearch.com/2018/10/08/keras-vs-tensorflow-which-one-is-better-and-which-one-should-i-learn/)
- [Deep Learning and Medical Image Analysis for Malaria Detection](https://www.pyimagesearch.com/2018/12/03/deep-learning-and-medical-image-analysis-with-keras/)
- [Transfer Learning for Image Classification using Keras](https://towardsdatascience.com/transfer-learning-for-image-classification-using-keras-c47ccf09c8c8)
- [Code a Smile Classifier using CNNS in Python](https://github.com/kylemcdonald/SmileCNN)
- [Natural Language Processing using scikit-learn](https://towardsdatascience.com/natural-language-processing-count-vectorization-with-scikit-learn-e7804269bb5e)
- [Code a Taylor Swift Lyrics Generator](https://towardsdatascience.com/ai-generates-taylor-swifts-song-lyrics-6fd92a03ef7e)
- [Mask detection using PyTorch Lightning](https://towardsdatascience.com/how-i-built-a-face-mask-detector-for-covid-19-using-pytorch-lightning-67eb3752fd61)

#### **Miscellaneous**
- [Build a Simple Interpreter](https://ruslanspivak.com/lsbasi-part1/)
- [Build a Simple Blockchain in Python](https://hackernoon.com/learn-blockchains-by-building-one-117428612f46)
- [Write a NoSQL Database in Python](https://jeffknupp.com/blog/2014/09/01/what-is-a-nosql-database-learn-by-writing-one-in-python/)
- [Building a Gas Pump Scanner with OpenCV/Python/iOS](https://hackernoon.com/building-a-gas-pump-scanner-with-opencv-python-ios-116fe6c9ae8b)
- [Build a Distributed Streaming System with Python and Kafka](https://codequs.com/p/S14jQ5UyG/build-a-distributed-streaming-system-with-apache-kafka-and-python)
- [Writing a basic x86-64 JIT compiler from scratch in stock Python](https://csl.name/post/python-jit/)
- Making a low level (Linux) debugger
  - [Part 1](https://blog.asrpo.com/makingalowleveldebugger)
  - [Part 2: C](https://blog.asrpo.com/makingalowleveldebuggerpart2)
- Implementing a Search Engine
  - [Part 1](http://www.ardendertat.com/2011/05/30/how-to-implement-a-search-engine-part-1-create-index/)
  - [Part 2](http://www.ardendertat.com/2011/05/31/how-to-implement-a-search-engine-part-2-query-index/)
  - [Part 3](http://www.ardendertat.com/2011/07/17/how-to-implement-a-search-engine-part-3-ranking-tf-idf/)
- [Build the Game of Life](https://robertheaton.com/2018/07/20/project-2-game-of-life/)
- [Create terminal ASCII art](https://robertheaton.com/2018/06/12/programming-projects-for-advanced-beginners-ascii-art/)
- [Write a Tic-Tac-Toe AI](https://robertheaton.com/2018/10/09/programming-projects-for-advanced-beginners-3-a/)
- [Create photomosaic art](https://robertheaton.com/2018/11/03/programming-project-4-photomosaics/)
- [Build the game "Snake" in the terminal](https://robertheaton.com/2018/12/02/programming-project-5-snake/)
- [Write yourself a Git](https://wyag.thb.lt/)
- [A Python implementation of a Python bytecode runner](https://www.aosabook.org/en/500L/a-python-interpreter-written-in-python.html)
- [Create a Voice assistant using Python](https://www.geeksforgeeks.org/voice-assistant-using-python/)

## **Rust**
- [Learning Rust by building a partial Game Boy emulator](https://jeremybanks.github.io/0dmg/)
- A Simple Web App in Rust
  - [Part 1](http://joelmccracken.github.io/entries/a-simple-web-app-in-rust-pt-1/)
  - [Part 2a](http://joelmccracken.github.io/entries/a-simple-web-app-in-rust-pt-2a/)
  - [Part 2b](http://joelmccracken.github.io/entries/a-simple-web-app-in-rust-pt-2b/)
- [Write an OS in pure Rust](https://os.phil-opp.com/)
- [Build a browser engine in Rust](https://limpet.net/mbrubeck/2014/08/08/toy-layout-engine-1.html)
- [Write a Microservice in Rust](http://www.goldsborough.me/rust/web/tutorial/2018/01/20/17-01-11-writingamicroserviceinrust/)
- [Learning Rust with Too Many Linked Lists](http://cglab.ca/~abeinges/blah/too-many-lists/book/README.html)
- Writing Scalable Chat Service from Scratch
  - [Part 1: Implementing WebSocket. Introduction.](https://nbaksalyar.github.io/2015/07/10/writing-chat-in-rust.html)
  - [Part 2: Sending and Receiving Messages](https://nbaksalyar.github.io/2015/11/09/rust-in-detail-2.html)
- [Writing a Rust Roguelike for the Desktop and the Web](https://aimlesslygoingforward.com/blog/2019/02/09/writing-a-rust-roguelike-for-the-desktop-and-the-web/)
- [Single Page Applications using Rust](http://www.sheshbabu.com/posts/rust-wasm-yew-single-page-application/)
- [Writing NES Emulator in Rust](https://bugzmanov.github.io/nesebook/)
- [Adventures in Rust: A Basic 2D Game](https://a5huynh.github.io/posts/2018/adventures-in-rust/)
- [Learning Parser Combinators With Rust](https://bodil.lol/parser-combinators/)
- [Build Your Own Shell using Rust](https://www.joshmcguigan.com/blog/build-your-own-shell-rust/)
- [Hecto: Build your own text editor in Rust ](https://www.flenker.blog/hecto/)
- [Command line apps in Rust](https://rust-cli.github.io/book/index.html)
- [Writing a Command Line Tool in Rust](https://mattgathu.dev/2017/08/29/writing-cli-app-rust.html)
- [Build your own Redis client and server](https://tokio.rs/tokio/tutorial/setup)


