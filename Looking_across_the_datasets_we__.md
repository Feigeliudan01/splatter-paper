Looking across the datasets we see that the Splat simulations are consistently good performers. On the Zeisel dataset both the zero-inflated simulations (Splat with dropout and Lun 2 ZINB) outperform their regular counterparts suggesting that this datasets is truly zero-inflated. Interestingly the Simple simulation is the best performer on the Engel dataset and best captures the variance and mean-variance relationship in the Tung dataset. This result suggests that the additional features of the more complex simulation may be unnecessary in this case or that other models may be more appropriate. The Splat simulations were least successful on the Camp cerebral organoid dataset. The complex nature of this data (many cell types) and the full-length protocol many have contributed to this poorer performance. In this situation the semi-parametric, sampling based model of the Lun 2 simulation may have an advantage, and was the best performer. The Lun simulation is consistently amongst the worst performing but, given that this model is largely similar to the others, it is likely due to the lack of an estimation procedure for most parameters rather than significant problems with the model. Most significantly we see that simulations perform differently on different datasets, emphasising the importance of trying different models and demonstrating their similarity to real datasets. The scDD also often differed significantly from the real data, particularly in library size and may benefit from the addition of fixed library sizes to the model. The Splatter framework makes these comparisons between simulation models straightforward.