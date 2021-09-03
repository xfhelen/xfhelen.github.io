---
layout: page
title: Unleashing the Energy-Saving Potential of Microservices
description: a project with no image
img:
importance: 4
category: AI&IoT
---

With ever-growing workloads in the cloud, it is critical to reinforce the capacity of APDC to meet the scale-out, emerging applications. Particularly, container and container orchestration have recently catalyzed the shift from monolithic applications to massive heterogeneous and loosely-connected microservices. This enables more scalability potentials at a ner-grained granularity. Meanwhile, this also requires us to re-think the challenges of accommodating convectional power management to microservice's features in APDCs.


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/9.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    One of the challenges is to match server-level power budget variation to fine-grained microservice heterogeneity.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/m1.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    It is difficult for current power management framework involving over microsecond-scale control latency to make informed power allocation decisions for microsecond-scale microservices.
</div>

Generally, when facing a myriad of short-lived tasks such as microservices, traditional power management needs to be re-examined at dierent layers to meet the new latency requirements.

