---
title: Funding
---

__[Contribute to theATL.social's operations via Patreon](https://patreon.com/theatlsocial) ❤️__

## Background

Mastodon server costs comprise payment for cloud-based servers, object storage, bandwidth, logging/monitoring, and other auxillary costs. As the number of users on a server increase, the cost per user decreases - an economy of scale.

## Current Costs

Monthly instance costs comprise:

| Description   |      Vendor      |  Monthly Cost |
|--------- | ------------- | ------|
| Security, Object Storage, DDOS Protection |  CloudFlare | $25 |
| Email Providers  |    SendGrid   |   $20 |
| Cloud-based Servers, Block Storage | DigitalOcean |    $90 |
| Container Repository + Docker Repo License | Docker Hub |    $7 |


### Why is this more expensive than a hosted service from masto.host, etc?

#### Queue Processing
- Maintaining a good level of service for existing active users and users moving their accounts from other servers requires considerable computing capacity for "queue processing." This processing occurs whenever users follow another user, receive a post from another server, and/or engage in any other action on the site. The costs of the existing infrasructure are similar in cost to the higher-tiered plans on Mastodon hosting services.
- Less queue processing capacity would result in considerable delays with user interactions on the site: statuses and posts from other services would take longer to receive, and posts from theATL.social would take longer to send.

#### Resiliency
- The Mastodon instance comprises of multiple servers, each operated separately to ensure that the failure of a single server will not "crash" the entire instance. This resiliency measure is not feasible on a hosted service.

#### Customization
- Hosted services offer constrained customization. theATL.social currently utilizes a number of custom settings and optimizations to enhance and secure the user experience that are not possible on a hosted instance.


## Full-Text Search (Elastic Search)

The server does not currently implement full-text search of posts, due to cost.

To implement a robust search capacity, approximately $100-125/month would be needed. These funds would purchase a two-node ElasticSearch cluster to provide the full-text service.

## Legal Organization

The server does not currently operate under a legal organization (e.g., a for-profit or non-profit corporation). Should the server continue expansion, an organization may be established under which the server operates. 