# Config SSH
My personal cloud coding environment powered by [Coder](https://github.com/cdr/code-server) and [Digital Ocean](https://www.digitalocean.com/).

## Setup your Digital Ocean environment
Create a droplet with the following options:
- Distribution: __Ubuntu 18.04.3 (LTS) x64__
- Plan:
    - __Standard__
    - __$40/mo__
    - __$0.060/hour__
        - __8 GB__ / 4 CPUs
        - __160 GB__ SSD disk
        - __5 TB__ transfer
- Datacenter Region: __Singapore__
- Additional Options:
    - [x] __IPv6__
- Authentication: __SSH Keys__
- Finalize and create
    - How many droplets: __1__
    - Hostname: _Choose whatever you want_

## Run Visual Studio Code
You must first have Docker installed before running the following command:
```
docker run -it -p 127.0.0.1:8080:8080 -v "${HOME}/.local/share/code-server:/home/coder/.local/share/code-server" -v "$PWD:/home/coder/project" codercom/code-server:v2
```

## Video Reference
There's also a [video](https://www.youtube.com/watch?v=N5WojMutddQ) that you can watch by __Fireship__.

## Warning
Remember to turn off the instance after you're done using it! It will be costly if you keep it running.
