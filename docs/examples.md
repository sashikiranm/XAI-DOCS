<!-- # IMPLEMENTING ARYA-xAI IMAGE CLASSIFICATION ON MNIST DATA -->

# MNIST DATA (INPUT)

We have used the MNIST character recognition dataset to demonstrate the Arya-xAI framework. The MNIST dataset of handwritten single digits between 0 and 9, consists of 60,000 small, square grayscale images with resolution 28×28pixels. A custom architecture, which contains most of the commonly used components such as convolutions and lstms, is designed for this data.

<p float = "left">
	<img src="../Images/fig1_input.png"  width="100">
	<img src="../Images/fig2_input.png" width="100">
	<img src="../Images/fig3_input.png" width="100">
	<img src="../Images/fig4_input.png" width="100">
</p>
<p float = "left">
	<img src="../Images/fig5_input.png"  width="100">
	<img src="../Images/fig8_input.png" width="100">
	<img src="../Images/fig9_input.png" width="100">
</p>


# NEURAL NETWORK USED 

<p style="text-align:center"> INPUT NETWORK ARCHITECTURE </p>
<p style="text-align:center">	<img src="../Images/input.png" width="400">
</p>				

<p style="text-align:center"> OUTPUT NETWORK ARCHITECTURE from Arya-xAI</p>
<p style="text-align:center">	<img src="../Images/output.png" width="400">
</p>				
# OUTPUT

## Default Mode

<p float = "left">
	<img src="../Images/fig1_bt.png"  width="100">
	<img src="../Images/fig2_bt.png" width="100">
	<img src="../Images/fig3_bt.png" width="100">
	<img src="../Images/fig4_bt.png" width="100">
</p>
<p float = "left">
	<img src="../Images/fig5_bt.png"  width="100">
	<img src="../Images/fig8_bt.png" width="100">
	<img src="../Images/fig9_bt.png" width="100">
</p>

## Contrastive Mode

 <p float="left">
 	<img src="../Images/fig1_bt_neg_full.png"  width="100">
 	<img src="../Images/fig1_bt_pos_full.png"  width="100">
 	<img src="../Images/fig2_bt_neg_full.png"  width="100">
 	<img src="../Images/fig2_bt_pos_full.png"  width="100">
 	<img src="../Images/fig3_bt_neg_full.png"  width="100">
	<img src="../Images/fig3_bt_pos_full.png"  width="100">
 </p> 


<p float = "left">
	<img src="../Images/fig4_bt_neg_full.png"  width="100">
	<img src="../Images/fig4_bt_pos_full.png"  width="100">
	<img src="../Images/fig5_bt_neg_full.png"  width="100">
	<img src="../Images/fig5_bt_pos_full.png"  width="100">
</p>


<p float = "left">
	<img src="../Images/fig8_bt_neg_full.png"  width="100">
	<img src="../Images/fig8_bt_pos_full.png"  width="100">
	<img src="../Images/fig9_bt_neg_full.png"  width="100">
	<img src="../Images/fig9_bt_pos_full.png"  width="100">
</p>

(Reference : BLUE - negative contrast , GREEN - positive contrast)



