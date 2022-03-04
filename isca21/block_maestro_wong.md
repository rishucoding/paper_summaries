## Title: BlockMaestro - Enabling Programmer-Transparent Task-based Execution in GPU Systems
Link: https://hodjat.me/pubs/BlockMaestro_ISCA21.pdf

### Problem: 
- Applications like FFT, Gaussian, GramSchm, etc contains many kernels, and thus they incur heavy overheads of kernel launches. Also, there is issue of underutilization of GPU because of sync required to resolve the data-dependency between kernels. 
- Currently, the problem is solved using task based models but this requires lot of programmer effort. So, there is a need of an alternative way which doesn't require programmer invovlement. 

### Motivation and Key Ideas: 
- An application consists of many kernels. A GPU Kernel consists of many Threads Blocks(TB) or CTA(cooperative thread arrays). A TB consists of many warps, and a warp is a group of 32 threads. ![image info](./images/appln_to_thread.png)
- TODO: data dependence pattern between kernels ![image info](./images/depd_graph.png)
- TODO: various execution models to limit kernel launches via prelaunching ![image info](./images/various_exec_models.png)
- TODO: command queue reordering ![image info](./images/reordering.png)
- TODO: block maestro high level design ![image info](./images/dgm_block_maestro.png)

### Important takeaways:
- What does BlockMaestro literally mean? 
- Connecting the dots ... Similarlity of Prelaunching with Prefetching







