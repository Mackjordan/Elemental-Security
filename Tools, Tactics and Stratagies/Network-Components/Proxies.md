# Proxy
A proxy server is an intermediary machine, between a client and the actual server, which is used to filter or cache requests made by the client.
* A proxy server can be single purpose - supporting one protocol, (e.g http) or multipurpose - supporting multiple protocols.

### Types of proxies
| Filter | Description |
|--------|-------------|
| Normal / Forward Proxy | The clients (Browsers) are configured to send requests to the proxy server. The proxy server receives the request, fetches the content and stores a copy for future use. The next time when another client requests for the same webpage, the proxy server just replies to the request with the content in its cache thus improving the overall request-reply speed.|
| Transparent Proxy | The same as forward proxy except that the client (browser) does not need to be configured. The proxy server resides on the gateway and intercepts requests. |
| Reverse Proxy | A reverse proxy, appears to the client just like an ordinary web server. The proxy caches all the static answers from the web server and replies to the clients from it’s cache to reduce the load on the web server. This type of setup is also known as a Web Server Acceleration.|
