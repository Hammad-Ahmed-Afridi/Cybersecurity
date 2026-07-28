# Try Hack Me
## Devsecops
- in devsecops path in try hack me most of the rooms were covered in security engineer path like ssdlc sdlc intro to devsecops but i will explain in simpler terms
  devsecops stands for development security operations these are procedures and practices that are carried out in software development lifecycle and now as it
  has security in it so it becomes secure software development lifecycle ssdlc it include automations continuous integration continuos delivery ci cd which
  include planning coding building testing releasing deploying and monitoring and loop goes on and this ci cd is automated to maximum for faster and more
  secure and more effiecient softwares deliveries devops became devsecops becasuse if security to be added from the beginning which is called shifting left
- in ci cd we have source code repo from which branching is done and changes are made to that branch and pushed by making a pull request and all of this is done
  using a version control system like git and the code repo is wither stored locally on private server or on cloud like github we also use gitlab and it also
  allows us to have our own private local gitlab server and in between this process of branching merging pushing their is a pipeline called ci cd pipeline
  which includes building testing and deploying and most of this is automated and have strict access controls and these systems are hardened and many tools are
  used for building testing deploying like in testing we use sast dast iast rasp we aslo have multiple encironments like dev env test enc pre prod env prod env etc 
- in devsecops we will comme across two most improtant terms called docker and kubernetes first discussing docker docker is a containerization platform like
  we use docker to create containers and what is container it is a package of software including code and its dependencies like a box having its code inside and
  all the dependencies that the code depends upon so that the entire app runs smoothly on any device it opens docker do not require any operating system as its
  own just like vm ddoes it uses the host os first we have docker engine which create docker containers from images that re defined in a docker file and then we
  have kubernetes which is an orchestration software which lets run multiple docker containers and manage them and setup more when needed or destroy when not needed
  we also have to enable and do security on docker and kubernetss as when using these technoloies they increase the attack surface for both docke and kubernetes
  we use yaml 
- we have cloud and on premise infrastructure which include servers which are than configured to provide services included compute network storage cloud is managed
  by cloud service provider like aws gcp azure etc and on prem is managed by the company itself for configuration managing and allocation dealocation of
  resources we use methods like manual ones which need to be configured and managed manually or automatically which is done using tools on prem infra is used
  for full control and data sovereignty and data protection against strict legal laws and regualations the automatic tool that is used for cloud resource management
  and creation is called terrraform and the language used is hcl hashicrop configuration language this language is cloud agnostic meaning it can be used in any
  csp and is also agentless meaning no agents need to be installed in a server or device to manage the resources in it and also it is a declarative language
  meaning the final desired state of the infrastructure is given by writing it in configuration file and the terraform core which manages all the actions 
