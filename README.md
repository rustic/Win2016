# Win2016
2016 Preview build with Packer and the Chocolatey package manager <https://chocolatey.org>

### To build:

This configuration builds the packer artifacts in a custom directory which can be set as an enviroment variable. To build the box run:

```
export PACKER_CACHE_DIR=$HOME/packer_cache
packer build -var-file=vars.json windows_server_2016.json
```

###To Do:
Find a more graceful way of specifying the output directory between the environment variable and vars.json. You could of course remove the references to these altogether and the output will be relative to where packer is run.

***
This repo borrows from works at:
[https://github.com/jacqinthebox/packer-templates] (https://github.com/jacqinthebox/packer-templates), 
[https://github.com/joefitzgerald/packer-windows](https://github.com/joefitzgerald/packer-windows) and 
[https://github.com/mwrock/packer-templates](https://github.com/mwrock/packer-templates).
