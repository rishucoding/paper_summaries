## Collecting Nvidia's thoughts on the new applications, and targetted hardware development strategies: 

### Key vocab: 
* generative AI
* accelerated computing

### Grace Hopper Architecture: 
* H100 features Grace CPU connected via NVLink (900 GBps) to Hopper GPU.
* New target applications: RecSys and LLMs.
* H100 NVL (dual-GPU NVLink) powers the LLMs inference. 
* H100 has a Transformer Engine (like a fixed functional unit) which accelerates GPT models. 
* For GPT-3, 4 pair of H100 NVL is 10x faster than HGX A100. (both have a total of 8 GPUs). 
* 

### Other notes: 
* NVDA and MSFT collaborating to improve the Microsoft 365 and Azure with efficiently plugging generative AI. 
* NVDA and AMZN collaborating to efficiently train the autonomous warehouse robots.
* NVDA working with ASML, TSMC, and SNPS to come up with 2-nm technology nodes.
* Rising adoption of H100 with major customers - oracle cloud infra, AWS EC2 UltraClusters P5 instances, Azure's ND H100 v5, Meta's Grand Teton AI supercomputer, OpenAI with Azure.
