---
layout: page
title: Cross-stack Power Anomalies 
img: /assets/img/50.jpg
importance: 2
category: System Optimization Techniques
---
Although conventional power optimization frameworks excel at managing power peaks incurred by normal users, they would fail to face abnormal attackers. This vulnerability exposes data centers to a new series of risks that we call power-oriented attacks. We have illustrated that it is feasible for adverse attackers to impact existing power budget management framework and disrupt normal operation by controlling the internal servers and VMs as well as sending malicious requests from an external internet.

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
    Like DDoS, server power-oriented attack could become a grave threat to aggressively provisioned data centers: On the left, Elusive Power Peak (EPP) attack is a server/VM-based power attack from inside, which often implements a three-phase attacking model. In the middle, conventioanl Denial-of-Service (DoS) attack cripples the targeted online service by sending massive requests through the Internet. On the right, Denial of Power and Energy (DOPE) attack is a new type of threat which overwhelms the power management system of data centers by sending selective traces from an external network.



</div>
<div class="row">
    <div class="col-sm mt-2 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/50-0.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Cross-layer power management for highly-availabile and highly-scalable data centers.
</div>

These power-oriented attacks impel us to think about how APDCs can maintain their benefits in a potentially insecure operating environment. To defend against power-oriented attacks, I propose to optimize traditional power management frameworks with cross-layer designs, such as orchestrating network balancers and power managers to prevent DOPE attack.
