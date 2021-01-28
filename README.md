# ECS Debezium POC Setup Notes
this is a setup note collected during the setup of mysql, debezium stack on aws ecs.

[ecs link](https://aws.amazon.com/ecs/)

[video tutorial](https://www.youtube.com/watch?v=kQBGbmrdYO4)

[debezium quick start](https://debezium.io/documentation/reference/tutorial.html#starting-mysql-database)

# Setup cluster

![image-20210127233119744](README.assets/image-20210127233119744.png)

Create cluster

![image-20210127233203251](README.assets/image-20210127233203251.png)

use 'Fargate'

![image-20210127233300610](README.assets/image-20210127233300610.png)

configure cluster, create

![image-20210127233455197](README.assets/image-20210127233455197.png)

finalize setup.



# Docker repository

![image-20210128003855544](README.assets/image-20210128003855544.png)

'view push command' to get push instructions

[working with mysql image docker](mysql/README.md)



# Task Definition

![image-20210128010255744](README.assets/image-20210128010255744.png)

![image-20210128011152511](README.assets/image-20210128011152511.png)

container config:

![image-20210128011035937](README.assets/image-20210128011035937.png)

![image-20210128011050161](README.assets/image-20210128011050161.png)

![image-20210128011235185](README.assets/image-20210128011235185.png)

create service

![image-20210128011352950](README.assets/image-20210128011352950.png)



![image-20210128011439050](README.assets/image-20210128011439050.png)



![image-20210128011538822](README.assets/image-20210128011538822.png)

![image-20210128011603859](README.assets/image-20210128011603859.png)

![image-20210128011615470](README.assets/image-20210128011615470.png)

