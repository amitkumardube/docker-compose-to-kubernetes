# docker-compose-to-kubernetes

3 ways we can move from docker compose to kubernetes

1. docker stack 
  - Only works with docker desktop
  - This doesn't create kubernetes files
  - This takes docker compose file as input and create resources in kubernetes without creating kubernetes files itself.
  - In order for docker stack to work with kubernetes, in docker desktop -> go to settings -> Kubernetes -> click **Deploy Docker Stacks to Kubernetes by default"** as shown in picture below
   ![image](https://user-images.githubusercontent.com/37042351/117619389-deac7200-b177-11eb-846e-fd8d63c19d56.png)

3. kompose
4. skaffold from google
