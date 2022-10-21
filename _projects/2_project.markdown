---
layout: page
title: Dedicated Profile of Multi-staged Microservice Application
img: /assets/img/microservice.jpg
importance: 2
category: Application Characterization Methods
---

With ever-growing workloads in the cloud, it is critical to reinforce the capacity of APDCs to meet the scale-out, emerging applications. Particularly, container and container orchestration have recently catalyzed the shift from monolithic applications to massive heterogeneous and loosely-connected microservices. This enables more scalability potentials at a microsecond-level granularity. Meanwhile, this also requires us to re-think the challenges of accommodating convectional power management to microservice's features in APDCs.

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
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/m1-0.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">

Current power management frameworks involve hundreds of milliseconds or even seconds of control latency, making it difficult to make informed power allocation decisions for microsecond-level microservices.


</div>

Generally, when facing a myriad of short-lived tasks such as microservices, traditional power management needs to be re-examined at different layers to meet the new latency requirements.

