# SynthSense

PTR Model Implementation 

The implementation of the PTR model is a combination of our own code and some of the code from the AutoBots architecture model1. We would like to also thank our TA Reynaheh Hosseininejad for the assistance she has provided with debugging our code.

 

Temporal (temp_attn_fn) 

First, we had to ensure that the tensors were sized properly and that the two tensors used were matching, so we had to permute one of them. Then, we had to manage the NaN values in the tensors. The positional encoding was written using the code provided from the PTR class, self.pos_encoder. Then, we applied the temporal attention for each time step. 

 

Social (social_attn_fn) 

The social attention function was implemented in the same way as the temporal function, but without the positional encoding. 

 

Forward (_forward) 

Here, we implemented a ‘for’ loop through the layers (L_enc) to obtain the temporal and social attention. 
