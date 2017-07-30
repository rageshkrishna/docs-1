page_main_title: PEM Keys
main_section: Platform
sub_section: Integrations
page_title: PEM integration

# PEM Key Integration

Available under the Integration Family: **Keys**

`PEM Key` Integration is used to connect Shippable DevOps Assembly Lines platform to VMs that allow PEM based auth. This is typically used to SSH in and then run activities on the machine. Tools like Terraform, Ansible need this to execute scripts on the machine

You can create this from the integrations page. This is the information you would require to create this integration

* **Name** -- friendly name for the integration
* **Key** -- Encrypted Key in PEM format

## Resources that use this Integration
Resources are the bulding blocks of assembly lines and some types of resource refer to Integrations by their name. The following Resources Types can created with `PEM Key` Integration 

* [integration]()

## Default Environment Variables
When you create a Resource with this integration, and use it as an `IN` or `OUT` into a Job that can execute user defined scripts, a set of environment variables are configured by the platform that may be useful to set the context before user defined scripts execute as part of the Job. These are variables available when this Resource is used

`<NAME>` is the the friendly name of the Resource

| Environment variable						| Description                         |
| ------------- 								|------------------------------------ |
| `<NAME>`\_INTEGRATION\_NAME   			| Name supplied in the integration |
| `<NAME>`\_INTEGRATION\_KEY				| PEM Key supplied in the integration |

## Further Reading
* GKE integration
* AWS integration
* runSH job
* runCLI job
* runCI job
* How to setup CI for my git repo

## TODO
| Tasks   |      Status    |
|----------|-------------|
| Hotlinking |  Open |
| Further Reading needs thinking|  Open |