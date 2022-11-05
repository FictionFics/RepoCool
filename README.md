# RepoCool

This repo will have the funtionality to save the perfect version of the Centralised project.

What is the idea of this Repository

- Create one cool infraestructure with interesting tools for house or small company. 
- Everything will be accessible only trough VPN connection using wireguard.
- The configuration is currently in docker, but maybe in the future move to k8 will be the evolution of this project.
- This project will be CI/CD and could have modifications depend on my personal time.
- All is in different containers interconnected, databases of the services are in a separate containers.

**Actual Services Inside the docker-compose.yml:**

- Bitwarden (Password manager) I used a Vaultwarden docker but I changed the database, the default image use SQL Lite, I changed for one that could escalate better (Postgress)
- Wireguard (VPN Server)
- Nging Proxy manager (Reverse Proxy or Load Balancer)
- Pi-hole (DNS PROXY) go here and add these lists of URLs into your pi-hole to increse the block adds experience: https://firebog.net/


**Future Services that I want to add:**

- Nextcloud (Your hosted cloud service)
- Keycloak (User manager and SSO tool)
- Rocket (Collaborating chat tool)
- Mail server? I need to think about this... Maybe I can die If I try it.


_I will update this document when I change something._


I am using my personal server with Ubuntu 20.04 LTS

This docker-compose.yml file create all the containers and dependencies between them, of course you should have docker installed on your machine and docker compose too. 

**IMPORTANT!**

I was able to access to all the services installed but when you are connected to the vpn, navegate to others things that are not these services will be blocked. I need to review properly the IPtables in the VPN to allow other connections.

