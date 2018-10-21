This repo will be for all the documentation we will need/have for the lab.

# Lab

<img src="https://www.49sd.com/content/images/2017/04/49sdLogo-1.png" alt="49th Logo" alight="center" height="300" 
width="300">

## What is it?

The lab is a place of education that 49th utilizes to create a safe and educational environment for new people to the 
ethical hacking club the [49th Security Division](https://www.49sd.com/) at UNC Charlotte.

## Why github?

We are going to be using github to store all the code we will be using for the infrastructure. This will allow people 
to contribute to the lab that want to in an opensource and educational fashion. The final say of if the information 
will get admitted or not will be up to a lab troll (definition link here). They are the keepers of the lab.

## What will be on here?
We have great plans for the lab, and plan to use a lot of devops tools to manage and control everything in the lab. The 
reason why is because [IaC](https://en.wikipedia.org/wiki/Infrastructure_as_Code) is an auditable and reproducible way 
to control your infrastructure, so that way other people can understand what is happening in your infrastructure and 
easily (or at least easier) assume responsibility of it with full understanding of what is happening.

## What devops tools will you use?
From the devops community we will we use a variety of tools:
- [terraform](https://www.terraform.io/) - used to control and manage the vCenter (vm) infrastructure
- [ansible](https://www.ansible.com/) - used to provision the vms infrastructure, this will be our configuration 
management tool.
- [vault](https://www.vaultproject.io/) - to manage password infrastructure for everything internal
- [packer](https://www.packer.io/) - this will build the vms that we will control with the tools above
- [jenkins](https://jenkins.io/) - will automate the packer builds so they stay up to date and other automation tasks
- [teamcity](https://www.jetbrains.com/teamcity/) - this will ensure code sanity/checking to make sure nothing is badly 
configured in our IaC
- [kubernetes](https://kubernetes.io/) - to orchestrate vulnerable environments for students to learn in

## What security/infrastructure tools will you use?
We will be using a whole host of security tools as well:
- Palo Alto Firewall - used to maintain the over aching network of the lab
- vCenter - used to host our vm infrastructure
- Splunk - used to aggregate logs and monitor internal traffic
- pfSense firewall - used to segment internal networks and simulate attack environments

## Who can help/be involved?
This is github and everything is opensource so anyone can help out with this. The majority of this will be done by lab 
trolls and lab minions (link to definition), as they will be in charge of approval processes to all official lab repos.
