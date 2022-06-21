# Infrastructure as Code

After you've mastered cloud computing and can manually operate on any cloud platform, the next step is to get started with [Infrastructure as code or configuration]. (https://learn.hashicorp.com/tutorials/terraform/infrastructure-as-code)

To master this phase, you can choose from a variety of programmatic or declarative languages/tools.

It is suggested that you understand the declarative language provided by the cloud platform on which you work (eg: ARM for azure, cloudformation for AWS, Google cloud deployment manager).
Then begin using [Terraform](https://www.terraform.io/) (as the most popular and widely used across all clouds)

There are numerous players with various purpose-built Declarative/programmatic languages that will require learning for various usecases. The guides on this page will exclusively cover opensource/commodity tools and technologies. Aside from that, there are numerous SaaS providers who enable continuous infrastructure through code with their own proprietary code. DSL (Domain specific language)

Categories include

## Cloud infrastructure provisioning and lifecycle management

The following is the bare essentials to learn for infrastructure as code and automation. This is needed for cloud provisioning and lifecycle management. You could choose a learning path of any one.

- [Terraform](https://www.terraform.io/)
- [Pulumi](https://www.pulumi.com/)
- [Azure Resource manager templates](https://docs.microsoft.com/en-us/azure/azure-resource-manager/templates/overview) and [Azure Bicep (Only for Microsoft Azure Cloud)](https://docs.microsoft.com/en-us/azure/azure-resource-manager/bicep/overview?tabs=bicep)
- [AWS Cloud-formation (only for AWS Cloud)](https://aws.amazon.com/cloudformation/)
- [GCP cloud deployment manager templates (only for GCP)](https://cloud.google.com/deployment-manager/docs)

Other low adoption tools exist as well, which is more just fun to experiment with rather than used full-fledge at production scale

- [Apache libcloud](https://libcloud.apache.org/)

There are also tools that can be used for more advanced approaches (eg: IaC GitOps through kubernetes [crossplane](https://crossplane.io/)).

## Application deployment, Configuration Management and infrastructure orchestration

A relatively more-wider and greyer scoped set of tools that will aid in system administration of large scale cloud setups. From managing servers, server configurations, application configurations and deployments.

The most widely adopted are the following

- [ansible](https://www.ansible.com/)
- [puppet](https://puppet.com/)
- [chef](https://www.chef.io/)
- [Saltstack](https://saltproject.io/)

There are lots of other configuration management tools, that can range from simple (eg: [cloudinit](https://cloudinit.readthedocs.io/en/latest/) to more expansive), but which is comparably much lesser adopted than the above 4.

## Security, Compliance and Governance

TBD

# Learning Paths

## Terraform

### What you will learn

- Expert in provisioning and managing infrastructure in any of the cloud platforms using Terraform
  - Creation, publishing and usage of modules in terraform
  - Manage multi-stack, multi-region, multi-environment setup in the cloud using terraform
  - Backend state management

### Time Commitment

Recommended Time:

- Starting from scratch to basic operational knowledge : _1 weeks_ (at 4 hours per day)

### Learning Paths

| complexity      | Material              |
| --------------- | --------------------- |
| `standard-path` | [hashicorp learn][1a] |

<!--Reference links in article-->

[1a]: https://learn.hashicorp.com/terraform

### Usecases Yardstick

- Try to complete the same [usecase](./learning-a-cloud.md#usecases-yardstick) ony using terraform
  - Develop modules for Network, databases, storage and compute separately
  - Assemble the modules to deploy the full stack
  - Provision and manage terraform state using a block storage (eg: blob or S3 buckets)
