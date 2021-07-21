# Home Assistant Unable to connect behind proxy
## For everyone also having this problem.

## In my case I am using a reverse Proxy with Apache to reach my HASS installation.
The problem I was seeing happened, because Apache does not forward WebSocket connections automatically.
Above is the .conf file that works for me.
If the problem should arise again **after** it worked make sure the path forwarded as a WebSocket connection is still correct.

*You may also need to install the wstunnel apache package!*
