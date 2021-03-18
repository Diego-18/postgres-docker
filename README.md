# postgres-docker
Docker postgres environment (Postgres, pgadmin)

# Prerequisites:

  Docker
  
  Docker-compose

# RUN:
  
  1. Create the directory at the following location: '/opt/postgres/config/postgresql.conf', '/opt/postgres/data', '/opt/shared_container'.
  
  2. Create a new network in which you will include the postgres container and pgadmin. 
      It is important that both are on the same network so that they can communicate with each other).
      
    docker network create --driver bridge network_bd
  
  3. Execute the following command in the folder where the Dockercompose.yaml file is located. 
    
    sudo docker-compose up -d  
    
    
@Diego-18
