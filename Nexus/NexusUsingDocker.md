-------------------------------------
#Installing Nexus Using Docker Image
-------------------------------------

Step 1. Firstly you need to setup docker using docker script.

Step 2. Downloading and running nexus Image:
   
   docker run -d --name nexus3 -p 8081:8081 sonatype/nexus3

   (Here 8081 is the default port of nexus)

    #sonatype/nexus3 is the docker image of nexus. Reference URL: https://hub.docker.com/r/sonatype/nexus3/

Step 3. Accessing and Loging In Nexus:

    1. You will see a login dashboard where you will find a path for getting access password:  sonatype-work/nexus3/admin.password

    2. Firstly go inside container (Since nexus is a container you will find this file there itself)

        $ docker exec -it <ContainerID> 

    3. Now go to this path and copy the password to login.
