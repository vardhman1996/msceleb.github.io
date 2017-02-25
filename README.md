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

### Quick Edit and Preview
Note that the cmd in step 3 normally takes 1-2 minutes as everytime it needs to setup the Jekyll environment from scratch.  

For quick edit and preview, you can run the following command by adding `bash` to the end.

```
docker run --rm --label=jekyll --volume=%cd%:/srv/jekyll -it -p 127.0.0.1:4000:4000 jekyll/jekyll:pages bash
```

Then you will be in a `bash` shell inside docker. You can run `jekyll serve` to launch the website, and view the webpage http://localhost:4000 in browser.

If you make any change to the website content, you can terminate `jekyll` by pressing `CTRL+C` in the docker, and relaunch it by running `jekyll serve`.