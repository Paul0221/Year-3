Maximum Likelihood Estimation (MLE) - write down the likelihood of a sequence of observations (e.g. 'HTTTHHHTTTTHHHT') and maximise the likelihood with respect to μ

This means the observations can be rearranged in any order without affecting the likelihood

Example:
		In ![[Pasted image 20231011170908.png]] we find the value of μ that maximises the likelihood, ![[Pasted image 20231011170956.png]] by:
		![[Pasted image 20231011171044.png]]
		This works out as: ![[Pasted image 20231011171137.png]]
		Therefore solving for μ: ![[Pasted image 20231011171226.png]]

Maximum Likelihood Estimation is prone to overfitting 

For example, if we observe 'HHH' (code 'T' = 0, 'H' = 1), ![[Pasted image 20231011171554.png]]

However, this implies that the best estimate for a future series of events is always heads which isn't right