# Real-time Streaming Chart Example

> A simple real-time streaming chart using [Smoothie Charts](https://github.com/joewalnes/smoothie), [Butterfly.Clients](https://github.com/firesharkstudios/butterfly-client) and [Butterfly.Web](https://github.com/firesharkstudios/butterfly-web)

You should see something like this after running the demo...

![Demo](https://raw.githubusercontent.com/firesharkstudios/butterfly-server/master/img/real-time-chart-demo.gif) 

Note this isn't just generating random data in the client.  The server is streaming real-time data to the client.

This example shows...

- A plain HTML/JS client subscribing to the Subscription API via the [Butterfly.Clients](https://github.com/firesharkstudios/butterfly-client) web client to receive updates on the "data-feed" channel and showing the values in a Smoothie Chart
- Implementing the Subscription API from [Butterfly.Web](https://github.com/firesharkstudios/butterfly-web) on the server

This example uses a plain HTML/JS client but the [Butterfly.Clients](https://github.com/firesharkstudios/butterfly-client) web client is vanilla javascript and can be used with any framework.

This example uses the [EmbedIO](https://github.com/unosquare/embedio) web server but [Butterfly.Web](https://github.com/firesharkstudios/butterfly-web) supports multiple web servers.

# Get the Code

```
git clone https://github.com/firesharkstudios/butterfly-server
```

# Run It

```
cd butterfly-server\Butterfly.Example.RealtimeStreamingChart\www
npm install
cd ..
dotnet run www
```

Now open a browser to http://localhost:8000/.

You can see the server code that runs at [Program.cs](https://github.com/firesharkstudios/butterfly-server/blob/master/Butterfly.Example.RealtimeStreamingChart/Program.cs). This is based on [Smoothie Charts Tutorial](http://smoothiecharts.org/tutorial.html) but changes the example to receive the real-time data from [Butterfly.Server](https://butterflyserver.io).

