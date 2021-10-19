# INPUT 

###### DATA

We have used the MNIST character recognition dataset to demonstrate the Arya-xAI framework. The MNIST dataset of handwritten single digits between 0 and 9, consists of 60,000 small, square grayscale images with resolution 28×28pixels. A custom architecture, which contains most of the commonly used components such as convolutions and lstms, is designed for this data.



![fig2_input](../Images/fig2_input.png)

![fig3_input](../Images/fig3_input.png)

![fig4_input](../Images/fig4_input.png)

![fig5_input](../Images/fig5_input.png)

![fig8_input](../Images/fig8_input.png)

![fig9_input](../Images/fig9_input.png)

​	Examples of input 



###### 												      	INPUT AND OUTPUT NETWORK

<img src="https://lh5.googleusercontent.com/9UnRaieyZs5GoBEGi1og8UUZ9OUgR7I-6JbK_HgrIyV6fYiutKS7cPYrtEnj57c2qZgWwL7fRp46WpH2gCGyfeJeYv2W5t_X9kg1QhAEnUyckTFJ_TJ-MJRu26bVnmM1Dbj01BIQ=s0" alt="img" style="zoom: 200%;" />



##### DEFAULT MODE OUTPUT

![](../Images/fig1_bt.png)

![fig2_bt](../Images/fig2_bt.png)

![fig3_bt](../Images/fig3_bt.png)

![fig4_bt](../Images/fig4_bt.png)

![fig5_bt](../Images/fig5_bt.png)

![fig8_bt](../Images/fig8_bt.png)

![fig9_bt](../Images/fig9_bt.png)



##### CONTRASTIVE MODE OUTPUT 

![fig1_bt_neg_full](../Images/fig1_bt_neg_full.png)

![fig1_bt_pos_full](../Images/fig1_bt_pos_full.png)

![fig2_bt_neg_full](../Images/fig2_bt_neg_full.png)

![fig2_bt_pos_full](../Images/fig2_bt_pos_full.png)

![fig3_bt_neg_full](../Images/fig3_bt_neg_full.png)

![fig3_bt_pos_full](../Images/fig3_bt_pos_full.png)

![fig4_bt_neg_full](../Images/fig4_bt_neg_full.png)

![fig4_bt_pos_full](../Images/fig4_bt_pos_full.png)

![fig5_bt_neg_full](../Images/fig5_bt_neg_full.png)

![fig5_bt_pos_full](../Images/fig5_bt_pos_full.png)

![fig8_bt_neg_full](../Images/fig8_bt_neg_full.png)

![fig8_bt_pos_full](../Images/fig8_bt_pos_full.png)

![fig9_bt_neg_full](../Images/fig9_bt_neg_full.png)

![fig9_bt_pos_full](../Images/fig9_bt_pos_full.png)

​	(Reference : BLUE - negative contrast , GREEN - positive contrast)



**Impact on pruning and model result assessment**

- For model pruning, current explainable approaches offer limited evidence on node/layer level importance in final prediction. The limits range from type of data to network architecture. Arya-XAI uses a unique approach to figure out the importance of each node/layer on the final prediction. This allows a much deeper explainability of the complex black box models for data scientists/researchers, allowing them to gauge which features have the most impact on the model decision. Explanations can be generated at a local level as well as a global level.
- Global level explanations can be used to study the overall model trend, data usage and identify possible improvements. Local level explanations are important for granular control over data usage and unit level performance of the network. Local level explanations not only help in analyzing model outputs for individual samples, they also help in establishing internal trends in any feature with respect to the decision. This facilitates in building feature-level decision boundaries and flag any adverse predictions. 