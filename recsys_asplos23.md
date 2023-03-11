## MP-Rec: Hardware-Software Co-Design to Enable Multi-Path Recommendation
### Link: https://arxiv.org/pdf/2302.10872.pdf
### Research Group: FAIR Meta, Harvard

### Details: 
* One line summary: ???
* Problem: Hybrid embedding representation sounds like a good idea, but not one hardware is suitable for all types. Eg: for a GEMM representation, it could be accelerated using TPU/GPU and thereby perform better than original table representation.
* New insights: 
    - Going beyond fixed embedding representations.Thinking about multiple embedding representations and their mapping to various hardware configurations.
    - Why? Recent research from Google Brain, and FAIR shows how to mathematically mimic tables using GEMM. 
    - Hybrid embedding representation is proposed but at the expense of more computation and memory needs -- PROBLEM
    - MP-Rec dynamically selects the embedding representation! 
* Imagination: 
    - In the embedding stage in DLRM, think of various offerings to do the embedding operation. We can pick based on the imposed constraints. (Fixed --> Flexibility)

* My questions: 
    - Is this a real problem or a synthetic problem? Because, how well is the idea of multiple embedding representation adopted in Meta?
    - The dataset picked falls in the super High Hot category. How would their work pan out for med/low hot situations? 
    - Model sizes are not-at-all representative of practical large models.
    - The CPU picked is too too old. Broadwell -- What is this? We have skylake, cascade lake, Ice lake, and then SPR now. Broadwell is 10 years old now! 
    - The GPU picked is also not representative. V100 -- we are about to have H100 come out, after A100(2020). Volta is 7 years old now! 
    - Picking old CPU/GPU seems biased to promote the case of using accelerators! 
    - Learning: How to train DLRMs using the TB/Kaggle datasets, and what kind of accuracies do we get? Comparing that with the pre-trained model! 

* References emphasized: 
    - Google Brain: Learning to embed categorical features without embedding tables for recommendation, KDD 21
    - FAIR: Tensor train compression for deep learning recommendation models, MLSys 21
    - FAIR: Sustainable ai: Environmental implications,challenges and opportunities, MLSys 21
