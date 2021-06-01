Configuration Files
This repo contains the different configuration files used to deploy the system on a Kubernetes Cluster
Additionally, it also contains the config files for the stress tests performed on the system

Kubernetes files:
backend.yaml
    Handles the deployment and service of Yggdrasil
heimdall.yaml
    Handles the deployment and service of Heimdall
room-repository.yaml
    Handles the deployment and service of Huginn
user-repository.yaml
    Handles the deployment and service of Muginn
odin.yaml
    Handles the deployment and service of Odin
database-pod.yaml
    Handles the deployment of the database
backend-config.yaml
    Handles the backend config of sticky sessions for the ingress and Heimdall service
coffeebreak-cetificate.yaml
    Handles the ManagedCertificate for the ingress in order to get HTTPS connection through Google
coffeebeak-ingress.yaml
    Handles the ingress configuration
redis-master.yaml
    Handles the redis master config
redis-slave.yaml
    Handles the redis slave config

Artillery Files
RoomRepo.yaml
    Stress tests the room repository, Huginn.
UserRepo.taml
    Stress tests the user repository, Muginn.
SocketStress.yaml
    Stress tests the socket server and room deployment, Heimdall