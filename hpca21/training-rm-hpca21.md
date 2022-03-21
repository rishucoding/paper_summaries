## CPU GPU Profiling for Training Recommendation Models

#### Hardware: 
![](./images/table-hw-config.png) 

#### Application properties: 
* Three models
* ![](./images/application_properties.png) 

#### Summary:
* CPUs are considered for training due to large memory capacity and bandwidth requirement coming from large embedding tables (TBs in size). 
* Optimizing the placement of EMB(embedding tables) happens is the key to performance. 

#### Main motivation for Heterogeneous Opportunity: 
*  ![](./images/cpu_vs_gpu1.png)
	* Right placement of EMB in various hardware: (showing optimal placement strategies)

*  ![](./images/placement_strategies.png)
	* Various strategies of placement: 
