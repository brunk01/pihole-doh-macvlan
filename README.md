I switched from a cable provider to fibre optic home internet and the new provider doesn't allow me to set a custom DNS server. To resolve it, I disabled the DHCP server on my provider's modem and I created this PiHole image that will take over DHCP duties as well as allow me to set the PiHole as the DNS lookup.

Credit where credit is due, I used this image for inspiration: [azamserver/pihole-doh ](https://hub.docker.com/r/azamserver/pihole-doh). I'm running a Pi3 in 32-bit mode so I changed that Dockerfile to use armhf vs amd64 and enabled DHCP in the docker-compose.yaml file
