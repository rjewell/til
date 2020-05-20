# BrowserSync in Docker

[BrowserSync](https://www.browsersync.io) is an incredibly popular frontend tool that, at it's most common and simplest, just refreshes your viewport
when it sees a file change to save you a click. 

[ustwo/docker-browser-sync](https://github.com/ustwo/docker-browser-sync) is a handy little dockerfile for running a static webserver via browsersync
in a container.

```
docker run -dt \
           --name browser-sync \
           -p 3000:3000 \
           -p 3001:3001 \
           -v $(PWD):/source \
           -w /source \
           ustwo/browser-sync \
           start --server --files "css/*.css"
```
