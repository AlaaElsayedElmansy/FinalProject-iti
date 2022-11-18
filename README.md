# prev
Graduation project is a fully infrastructure on google cloud platform (GCP) where we could deploy web app on it using DevOps tools like ( kubernates - Docker - jenkins ).

## 1-Infrastructre
Using Terraform we create infrastructure modules and used it to built infrastructure that shown blow on GCP
1- vpc

    one VPC

2- subnets

Two subnet

    one subnet for managment

    one subnet for restricted

3- managment VM

    VM contain gcloud and kubectl to deploy kubernetes

    connect command of cluster to setup the kubeconfig of cluster in vm to deal with cluster

4- firewall

    allow connect by IAP only

4- GKE

    one cluster and 2 nodes

    private cluster and nodes

    authorized network with subnet range of managment-cidr

6- service account

Two Service account

    one for VM

    one for GKE

### 2- Deployment

1- deploy jenkins

    the offical Image of Jenkins

2- deploy jenkins slave

    build Image of base ubnutu conatin:

        Docker

        Kubectl

        gcloud

        helm

        Java

3- apply volumes to mount Data

4- namespace

5- service account
