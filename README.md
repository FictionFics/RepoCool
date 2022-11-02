# RepoCool

This repo will have the funtionality to save the perfect version of the Centralised project.

What is the idea of this Repository

- Create one cool infraestructure with interesting tools for house or small company. 
- Everything will be accessible only trough VPN connection using wireguard.
- The configuration is currently in docker, but maybe in the future move to k8 will be the evolution of this project.
- This project will be CI/CD and could have modifications depend on my personal time.
- All is in different containers interconnected, databases of the services are in a separate containers.

Actual Services Inside the docker-compose.yml:

- Bitwarden (Password manager) I used a Vaultwarden docker but I changed the database, the default image use SQL Lite, I changed for one that could escalate better (Postgress)
- Wireguard (VPN Server)
- Nging Proxy manager (Reverse Proxy or Load Balancer) 


Future Services that I want to add:

- Nextcloud (Your hosted cloud service)
- Keycloak (User manager and SSO tool)
- Rocket (Collaborating chat tool)
- Mail server? I need to think about this... Maybe I can die If I try it.


I will update this document when I change something. 
