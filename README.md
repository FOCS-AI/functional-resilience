# functional-resilience
Combining Node with Functions in Optical Network Topology for Resilience under attack and recovery

# Topology and Function: Integrated Resilience of Optical Networks under Attack and Recovery

Functional distribution over an optical network refers to the spatial allocation of network functions (e.g., core routers, data centers, IXPs) across the physical nodes of the topology. Functional distribution captures what role each node plays in delivering services.

<img width="1036" height="440" alt="image" src="https://github.com/user-attachments/assets/09ee8034-463b-45f4-9cc2-921b1303b0e3" />

## Node -> mapped to a set of functions -> functions have tunable importance weights 
This is done using a custom simulator where distributed and centralised function placements are generated
Weights are assumed here based on relative importance of these functions within the network and can be tuned

<img width="500" height="800" alt="image" src="https://github.com/user-attachments/assets/74b52c78-4d89-45d8-94fa-25170ffcd594" />


## Do we need new metrics for functional resilience? 

Existing topological metrics fail to capture service degradation due to the assumption of homogeneous placement of network functions. We propose resilience metrics
that fill this gap and validate them on large-scale networks (USA, India, UK)

<img width="3008" height="734" alt="image" src="https://github.com/user-attachments/assets/3e5f4828-1685-4688-94f7-7e71d6990444" />

## Is topology alone sufficient to quantify network resilience, or must resilience be understood through the degradation of functions and services it supports? 

Existing topological resilience metrics remain of limited operational value for three reasons: 
- (a) no notion of service continuity, 
- (b) assume all nodes are homogeneous whereas diverse function placements make them heterogeneous in nature, and 
- (c) cannot differentiate between a topology with two different placements of network functions. 

In this paper, we develop functional resilience metrics based on two operator-relevant dimensions (i) **service continuity** and (ii) **service coverage** evaluated under probabilistic node attacks and recovery. We present both per-function resilience metrics, which provide diagnostic insight into individual service vulnerabilities, and network-level indicators to assess overall system resilience. 

Empirically, we show 
- (i) topological metrics remain unchanged across contrasting placements; 
- (ii) they decay faster than functional metrics, which reveals a premature-collapse bias; and 
- (iii) during recovery, functional resilience is contingent on the site-recovery sequence.

<img width="2530" height="940" alt="image" src="https://github.com/user-attachments/assets/9498650a-e138-468a-a3af-95da7b2235dd" />

## Functional Resilience Enables Intelligent and Secure Network Design and Planning

Functional resilience depends on the physical topology and on how network functions are heterogenously distributed across nodes. These metrics are actionable and enable operators to: 
- (a) diagnose whether vulnerabilities originate from topological constraints or suboptimal placement of functions over nodes, 
- (b) make informed cost-resilience trade-offs between centralised and distributed placements and 
- (c) identify how each function contributes to aggregated network resilience. 

<img width="1114" height="339" alt="image" src="https://github.com/user-attachments/assets/5c6e7260-74af-4013-b6e6-0c41b96298e1" />


Our validation on three large-scale optical networks (USA, India, UK) using our proposed service continuity and coverage metrics shows: 
- (i) distributed function placement improves resilience by 13–30% over centralised architectures; 
- (ii) topology-based metrics underestimate service survivability and 
- (iii) distributed placements exhibit higher resilience but slower recovery, revealing an operational trade-off.
