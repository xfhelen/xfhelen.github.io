---
layout: page
title: Hybrid Energy Backup Architecture 
img: /assets/img/IPAD_arch.JPG
importance: 2
category: Infrastructure Reconfiguration Mechanisms
---
Energy storage devices (e.g., batteries) are critical components for high-availability data center infrastructure today. Without resilient energy management of these devices, existing power-hungry data centers are largely unguarded targets for cyber criminals. Particularly for some of today’s scale-out data centers, power infrastructure oversubscription unavoidably taxes the data center’s backup energy resources (i.e., UPS), leaving very little room for dealing with power emergency. As a result, an attacker could manipulate the computing system to generate peak power demand and disrupt power-constrained server racks. This study aims at protecting data centers from malicious loads that seek to drain precious energy backup, overload server racks and compromise workload performance. We term such load as Elusive Power Peak (EPP) and demonstrate its basic three-phase attacking model. To defend against EPP, we propose IPAD, a remediation solution build on integrated software and hardware mechanisms. IPAD not only increases the attacking cost considerably by hiding vulnerable server racks from visible power peaks, but also strengthens the last line of defense against hidden power spikes with fine-grained power control strategy. We show that IPAD can effectively raise the bar of power-related attack, with reasonable design overhead.

</div>
<div class="row">
    <div class="col-sm mt-2 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/EPP_Attack.JPG' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Demonstration of the three-phase power attack, i.e., EPP Attack model.
</div>

Our IPAD design creates a hybrid energy backup pool for managing complex power anomalies. It exploits the energy stored in both batteries and super-capacitors. The batteries form a virtualized energy backup pool called virtual DEB (vDEB). The supercapacitors form a micro energy backup pool called micro-DEB (μDEB). The vDEB module aims at protecting data centers from a brute visible peak attack in the Level-1 emergency state. The vDEB design intends to defend against a more sophisticated hidden spike often seen in the Level-2 state.

</div>
<div class="row">
    <div class="col-sm mt-2 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/IPAD_arch.JPG' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    The IPAD architecture. In the figure it shows the deployment of three critical components, i.e., vDEB, uDEB, and SPS module.
</div>

