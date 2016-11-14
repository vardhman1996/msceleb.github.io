# MS-Celeb-1M: Challenge of Recognizing One Million Celebrities in the Real World
### Introduction
This repo is for maintaining the website of http://msceleb.org hosted on Github Pages.  
### Installation (on Windows)
1. Install Docker for Windows  
2. Clone this repo to a local folder  
   ```
   git clone https://bitbucket.org/leizhangcn/msceleb
   ```
3. Go to the repo local folder, and run docker:  
   ```
   docker run --rm --label=jekyll --volume=%cd%:/srv/jekyll -it -p 127.0.0.1:4000:4000 jekyll/jekyll:pages
   ```
4. Test the website in browser: http://localhost:4000  
