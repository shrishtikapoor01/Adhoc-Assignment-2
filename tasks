TASK-1:
Create 100 containers 25 each of alpine, fedora, centos, java which runs forever using python script.
Python Code:

import os
for num in range(1,101):
	if num<=25:
		os.system("docker run -itd --restart unless-stopped --name adhocnw{} alpine".format(num))
	elif num<=50:
		os.system("docker run -itd --restart unless-stopped --name adhocnw{} fedora".format(num))
	elif num<=75:
		os.system("docker run -itd --restart unless-stopped --name adhocnw{} centos".format(num))
	elif num<=100:
		os.system("docker run -itd --restart unless-stopped --name adhocnw{} java".format(num))
os.system("docker ps")


TASK-2:
Using combination of Docker and OS commands to get list of Names,Created of all containers and store them in a list.
        .
docker ps -a --format "table {{.Names}}\t{{.CreatedAt}}" > container_info.txt
cat container_info.txt


Task-3:
Creating custom docker image containing firefox as parent image.

No Docker intalled locally.


Task-4:
Using Task1, getting RAM and CPU consumption from 100 100 containers to store in a text file.

docker stats --all --no-stream --format "table {{.Name}}\t{{.CPUPerc}}\t{{.MemUsage}}\t{{.MemPerc}}" > sk.txt
cat sk.txt
