## Learning a cloud

Many of the key features are consistent across all cloud platforms. So it is less vital to be concerned about whatever platform to begin with than to begin and build expertise in the foundations that are transferrable across.

_pre-requisistes_ : Good understanding of "what is cloud computing" that can be found [here](./cloud-computing.md)

### Time Commitment

Will recommend picking one cloud platform and understanding all the fundamental services it provides, do some lab exercises and try to deploy your own application

_Recommended time:_

- Existing knowledge transferring from another cloud: _1 week_ (at ~ 3 hours per day)
- Starting from scratch to basic operational knowledge : _3 weeks_

### What you will learn

Working knowledge in the following with, setup and operational knowledge of the following on any cloud platform

- Networking, connectivity and security

  - Understanding of the OSI model
  - understanding of virtual networks, subnets, routing, public, private, DNS, gateways
  - Network firewalls (firewalls, nsgs, layer 4-7 protection, DDOS)
  - Edge (DNS, certificates, protection, WAF, CDN) and traffic management

- Compute, Application runtimes, containerised, serverless workload (Webapps, functions, lambdas)

  - configuration, setup and protection of application on the runtimes'
  - setup, management and lifecycle of storage solutions (blob, block, s3)

- Databases and Analytics

  - Databases/storage/cache as service (postgres, sql, redis, cosmos, dynamo)
  - Analytics services, usage.

- Core architectural components, composition and topology

  - Regions, availability zones, geo-redundancy, resilience setup
  - organisation and management (subscriptions, organisations, resource managers)
  - Best practices, resiliency, cost-efficiency and optimisations
  - Compliance and Governance, management policies

- Identity, Access management and governance
  - user, roles, permission management, management policies, managed identities
  - Understanding on AzureAD, conditional access
  - types of accounts (application types etc)

### Learning Paths

| cloud | complexity                              | Material                      |
| ----- | --------------------------------------- | ----------------------------- |
| azure | `standard-path` : one week              | [Azure Fundamentals][1a]      |
| azure | `youtubecrash-course` : theory in a day | [Azure fundamentals][1b]      |
| azure | `hands-on-practice` : couple of weeks   | [Azure Fundamentals labs][1c] |

<!--Reference links in article-->

[1a]: https://docs.microsoft.com/en-us/learn/certifications/azure-fundamentals/?tab=tab-learning-paths
[1b]: https://www.youtube.com/watch?v=NKEFWyqJ5XA
[1c]: https://github.com/MicrosoftLearning/AZ-900T0x-MicrosoftAzureFundamentals/tree/master/Instructions/Walkthroughs

### Usecases Yardstick

- Try out this or your variabtion of [this](https://acloudguru.com/blog/engineering/cloudguruchallenge-your-resume-in-azure) exercise
  - Any MVC style application deployed on azure/AWS
    - use a serverless compute
    - attach it to a virtual network and protect the network
    - expose it to the internet with custom DNS and WAF/firewalls
    - manage traffic across multiple regions
    - provision a database and storage account for the app to access using identity
