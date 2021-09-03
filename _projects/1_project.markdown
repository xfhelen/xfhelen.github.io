---
layout: page
title: Power-/Energy-related Attacks
description: a project with a background image
img: /assets/img/12.jpg
importance: 1
category: Data Center
---
Although conventional power optimization frameworks excel at managing power peaks incurred by normal users, they would fail to face abnormal attackers. This vulnerability exposes data centers to a new series of risks that we call power-related attacks. We have illustrated that it is feasible for adverse attackers to impact existing power budget management framework and disrupt normal operation by controlling the internal servers and VMs as well as sending malicious requests from the external Internet.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/1.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/3.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/5.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Power-oriented attacks: On the left, Elusive Power Peak (EPP). Middle, Power Grab (PG). On the right, Denial of Power and Energy (DOPE).
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/50.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Cross-layer power management for highly-availabile and highly-scalable data centers.
</div>

These power-oriented attack impel us to think about how APDC can maintain their benets in a potentially insecure operating environment. To defend against power-related attacks, I propose to optimize traditional power management frameworks with cross-layer designs such as coordinating the network balancer and power manager to prevent the DOPE.