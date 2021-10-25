

# ***Welcome to Arya XAI (Explainable-AI)***


At Arya.ai, we recently released a new framework - ‘Arya-XAI’ to simplify DLOps in production. Arya-XAI(short for Arya-Explainable AI) enhances the credibility of the predictions of your DL model by generating new and simple explanations (pertaining to the generation of these predictions) in real time as required by various stakeholders. 
This is the tutorial-first mode of operation for Arya-xAI and it also illustrates the capabilities of the framework.

# **Current approaches to Explainable AI and their challenges**

Current approaches to explain black-box DL models are heavily reliant on specific data types and network components, both of which severely limit their applicability to a diverse range of use-cases and novel network architectures. This poses challenges to understand or explain true-to-model functioning(that takes into account the internal design of the model). However, models like SHAP, LIME, Integrated Gradients etc. use a **permute-and-predict** approach to explain the model functioning. While the approaches do offer approximate explanations of how a DL model works on the input to ultimately yield the output, unfortunately these are understandable only by an AI expert. Unlike the existing models such as SHAP and LIME which do not take the internal structure of a network into account to explain its working, the Arya-XAI framework decodes explanations by computing weightage of each feature together with the node-level weightages for a given neural network architecture, referred to as **true-to-model** feature and node-level weightages respectively. The framework not only improves reliability on DL models substantially, but also offers easy-to-understand reasons behind the outcome. 