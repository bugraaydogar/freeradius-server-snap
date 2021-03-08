# Freeradius Server Snap

This is a snap of freeradius-server. You can get more information about it in the link below.
https://freeradius.org/

## Build
Clone the repo and run the following command.
`snapcraft --use-lxd`

## Installation
You can install the snap package that you built with
`snap install <nameofthesnap> --dangerous`
Alternatively, you could install from store by using
`snap install <TBD>`


## Configuration
Freeradius-server uses the default configuration. However, you could change clients.conf and users configurations by using the following commands;
`snap set freeradius-server clients="content of your clients.conf file"`
`snap set freeradius-server users="content of your users file"`

Hint: You could use;
```sh
clients=`cat <pathofyourfile>`
snap set freeradius-server clients="$cmd $clients"
```

## Run
Freeradius-server is a deamon that starts automatically by using the default configuration.

To print freeradius-server daemon logs:
`snap logs freeradius-server -f`

To stop the server:
`snap stop freeradius-server`

## Enjoy

and provide feedback ;)




