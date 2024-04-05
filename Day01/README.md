# Terraform interview questions for DevOps

1 - **What is Terraform?**

Terraform is an open-source tool that allows you to create, update, destroy, and version your infrastructure

---

2- **What are the two key components of Terraform?**


The two key components of Terraform are: Terraform core and Terraform pluggins

  - Terraform core : monitors the reading and interpolation of configuration files, resource plan executions, state management features, and resource graphs

  - Terraform pluggins: define resources for specific services, including initializing the libraries used to make API calls and authenticating infrastructure providers

  ---

  3- **Define IAC**
  Infrastructure as Code allows you to build , change , and manage your infrastructure through coding instead of manual processes

  ---

  4- **What are the most useful Terraform commands?**
  
  The most useful Terraform commands are: terraform init( initializes the current directory) , refresh (refreshes the state file), output(views Terraform outputs) , plan(a dry run to see what Terraform will do) , destroy(destroys what has been built by Terraform) , validate( validates the configuration files in a directory) , and apply( applies the Terraform code and builds infrastructure)

  ---

  5 -  Explain the difference between declarative and imperative approaches in  infrastrure provisioning

  In declarative provisioning, we define the desired end state without specifying the steps to reach that state. Example: Terraform. Although in imperative provisioning, we have to specify explicitely the intructions or commands to perform each step of the infrastructure provisioning. Example: Ansible

  ---

  6 - How does Terraform maintain the idempotency of resource provisioning?

  Terraform ensures idempotency by maintaining a state file that keeps track of the resources it manages. While runing Terraform apply, Terraform compares the Desired state described in the configuration file  with the Current  state (state file). Based on the comparison, it determines the necessary actions to reach the Desired state and applies changes to only the part that required changes
