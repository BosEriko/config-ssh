# Config SSH
My personal cloud coding environment powered by [Coder](https://github.com/cdr/code-server) and [Google Cloud](https://cloud.google.com/).

## Setup your Google Cloud environment
Create a [VM instance](https://console.cloud.google.com/compute/instancesAdd) under Compute Engine.
- Name it however you want
- Region should be __asia-southeast1 (Singapore)__ and the zone should be __asia-southeast1-a__
- Machine family should be __General-purpose__
- Machine series should be __N1__
- Machine type should be __Custom__ with __4 cores (vCPU)__ and __4gb memory__
- Do not deploy container Image to the VM instance
- Boot disk should be __Ubuntu 18.04 LTS__
- Do not change the configuration of __Identity and API access_
- Set the firewall to allow both HTTP and HTTPS traffic