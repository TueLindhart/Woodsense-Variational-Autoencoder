# Woodsense-Variational-Autoencoder


It can be challenging in an unsupervised setting to train andevaluate a deep learning model to detect outliers. This appliesespecially if the detection of outliers is based on a predictionor reconstruction error since you risk training the model onthe outlier data and hereby learning it to predict it.  This pa-per investigates if a Variational Autoencoder can be used tolearn  the  underlying  latent  distribution  of  multivariate  dataprovided  by  Woodsense  and  hereby  learn  to  detect  outliersand to generate ’normal’ data which other outlier detectionmodels  can  be  trained  upon.    The  model  ended  up  beinga Conditional Importance Weighted Autoencoder named theWoodsense Variational Autoencoder (WVAE) which can gen-erate data conditioned to the time of day and year. The modelseems to learn a representative latent space where ’normal’data can be sampled from the regions of high probability andoutlier data can be sampled from the regions of low probabil-ity.  However, it was also found that the ability of the modelto generate coherent multivariate data is limited to the timewindows of which it is provided in the training of the model.

*NOTE: Training data is not provided due to it being confidential for Woodsense A/S.*

**Content**

- Conditional RNN IWAE- Final.ipynb
  - The notebook preprocesses the data for training, defines the model, train the model and visualises the results. 
- RNNIWAE_input_w_c_32_1_layer_0_p_k_10_step_1_beta_0.015
  - The torch state dict of the last trained model of which visualizations are made. 

