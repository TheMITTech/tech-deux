# Tech Deux (WIP)

A "modern" rewrite of the previous [Ruby-based thetech.com site](https://github.com/TheMITTech/thetech.com); we're so back...

**This assumes you’re running on Windows, if you are using Linux/MacOS things will differ somewhat but links should have alternative options**  
1\. ***Download node.js and npm libraries*** through some method, recommended one below  
Libraries’ [docs](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) suggest using nvm-windows packager for Windows, you’re free to do whatever  
Version 1.2.2 as of 6/26/2026

2\. ***Download pnpm*** through some [method](https://pnpm.io/installation), I did npm way but up to you

3\. I would highly recommend doing the Astro [tutorial](https://docs.astro.build/en/tutorial/0-introduction/) to understand intuitively how Astro.js, our framework of choice, works and why it was chosen for this project.   
TLDR: content-driven optimizations mean very fast loading, and component-based design mean building out is supported by already-made modular components, and supports Typescript

4\. **Git clone** the [repository](https://github.com/TheMITTech/tech-deux)

5\. **cd** inside the now cloned repository, and run **pnpm install** to install dependencies.

6\. To start Astro development server, run **pnpm run dev** and open at [http://localhost:4321/](http://localhost:4321/) 

You should now be ready to start development of thetech.com’s “modern” rewrite.

**Adding changes to the repository**

TL;DR: First make a branch. Commit to the branch. Push the branch. Go to github page, open a pull request. Add/send to Techno Director (currently Rene Ramirez) to review

Steps:  
Run these commands:   
\- git add .  
\- git checkout \-b {branch name}  
\- git commit \-m {message}  
\- git push origin {branch name}  
after everything above, go to the repo, click compare & pull.   
add long\-burrito as a reviewer on the right side of the page  
Notes:  
branch name format: feature\_version  
message: some useful message  
long\-burrito is username of current Techno Director
