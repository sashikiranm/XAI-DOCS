### **How does Arya-xAI work?**

Arya XAI currently has two modes of operation known as default and contrastive mode which are demonstrated through the following use-cases respectively:

- Network Analysis: In this mode, there is a single,positive significance value that is propagated in proportion to the contribution of each unit. This can be used to prune the underutilized parts of the network and modify the saturated ones. This is also helpful in reducing or enhancing the input features. 

- Decision Analysis: In this mode, there are dual significance values which can be either negative or positive depending on the relative contribution of any unit to the decision. This is helpful in providing explanations regarding the corresponding input features that are positively/ negatively affecting the decision .

  

  The procedure for significance/relevance calculation is as follows:

1. From the model weights and architecture construct a graph with output nodes as roots and input nodes as the leaves.
2. The propagation starts at root and proceeds in breadth-first manner to avoid re-processing of any node.
3. The propagation completes when all the leaves(input nodes) have been assigned relevance. 
4. For the default mode, any loss of relevance during propagation is due to network bias. However, network bias is ignored for relevance computation in the contrastive mode.
5. The relevance of a single sample represents local importance. For global importance, the relevance of each feature can be aggregated after normalization on the sample level. 