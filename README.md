# docker-compose-to-kubernetes

3 ways we can move from docker compose to kubernetes

1. docker stack 
  - Only works with docker desktop
  - This doesn't create kubernetes files
  - This takes docker compose file as input and create resources in kubernetes without creating kubernetes files itself.
  - In order for docker stack to work with kubernetes, in docker desktop -> go to settings -> Kubernetes -> click **Deploy Docker Stacks to Kubernetes by default"** as shown in picture below
   ![image](https://user-images.githubusercontent.com/37042351/117619389-deac7200-b177-11eb-846e-fd8d63c19d56.png)

2. kompose (https://kompose.io/)
  - command to use is kompose convert with different flags
  - flags are
      - --file  - to pass different file other than default docker-compose.yml.
      - --out - to provide the output directory to save files to.
      - --stdout - to provide the output to standard output.
      - --help - to check available options ( help ).
      - --replicas - to adjust the number of replicas for the deployment. Default is 1.

3. skaffold from google
