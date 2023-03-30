# Ruby Websocket Client Example

This shows a quick way to connect to a socket, subscribe to a channel, and receive messages.  To run:

````zsh
./bin/bundle
cp .env.example .env
````

And fill out the two values in the new `.env` file:

1. **SOCKET_URI** [required]: URL to connect to
2. **CHANNEL_ID** [required]: Channel ID to subscribe to for updates

Once the `.env` configuration file has been filled out, run:

````zsh
./bin/bundle
./bin/client
````

This will install all dependencies and launch the client which will open up a socket and subcribe to the channel.  All messages from the server should now be emitted to the terminal.
