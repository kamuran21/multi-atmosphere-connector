# Multi Atmosphere Connector

Multi atmosphere connector is designed to create multi web socket connections thanks of Atmosphere JS. There two options to create any web socket connection. The first one is Atmosphere JS self the second one is using Atmosphere JS as a JQuery plugin.

# Using with Atmosphere JS self
Import atmosphere.js in your project. Select your package manager to install atmosphere.js
Npm :
<code>npm install atmosphere</code>

Bower :
<code>bower install atmosphere</code>

#Using with Atmosphere JS as JQuery Plugin
Import JQuery and Atmosphere JS jQuery plugin to your project.
Npm :
<code>npm install jquery atmosphere-jquery</code>

Bower :
<code>bower install jquery atmosphere-jquery</code>

#Install Multi Atmosphere Connector
Npm :
<code>npm install multi-atmosphere-connector</code>

Bower :
<code>bower install multi-atmosphere-connector</code>

#Usage

<b>For Single connection</b>
<code>
var socketConnection  = new AtmosphereConnector();
socketConnection.request.url = 'https://echo.websocket.org';
socketConnection.connectSocket();
socketConnection.socket.push('This is the single web socket connection');
</code>

<code>
var socketConnection1  = new AtmosphereConnector();
socketConnection1.request.url = 'https://echo.websocket.org';
socketConnection1.connectSocket();
socketConnection1.socket.push('This is the first web socket connection');

var socketConnection2  = new AtmosphereConnector();
socketConnection2.request.url = 'https://echo.websocket.org';
socketConnection2.connectSocket();
socketConnection2.socket.push('This is the second web socket connection');

socketConnection1.closeSocket();
socketConnection2.closeSocket();
</code>
