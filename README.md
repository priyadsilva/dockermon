# dockermon
docker-compose to monitor containers

Please create a docker compose configuration which will run 'AT LEAST' the following containers.

Prometheus
Alertmanager
NGINX
A frontend should be available for each of these services on the localhost.

Configure the above system in such a way so as when the NGINX container is down, this is registered in the Prometheus system, which will then send an alert to Alertmanager. This alert should be displayed on the Alertmanager UI. You do not need to configure any routes from the Alertmanager to any other systems such as email or slack.

You may configure the system in any way you like, you can use additional containers if required.

SOLUTION:

option1 is implemented using nginx-prometheus exporter. 

option2 is implemented using using cadvisor.
