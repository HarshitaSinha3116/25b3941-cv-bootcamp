# CV Bootcamp
## Q1
The confusion matrix points out that automobile and truck well as cat and dog are the class pairs that get mixed up the most. Deer and horse and airplane and ship also get mixed up a lot. These groups look alike so they are hard to tell apart. This means that mistakes, by labelers usually happen when the classes look similar not just by chance.

## Q2
Memorization begins around epoch 21. The training accuracy for images that are correctly labeled keeps going up. At the time the accuracy for images that are mislabeled starts to go up slowly. The noisy validation accuracy reaches its point of 55.62% at epoch 31 and then mostly goes down. This shows that the model starts to learn the labels. Also the performance, on the validation data stops getting better. Because of this epoch 31 was chosen for stopping.

## Q3
Cross-validated loss (cv_loss) was used to find images that might have labels. Images that have a cv_loss are more likely to have labels that do not match what the model predicts.. Sometimes even images, with the correct labels can have high loss because they are hard to classify. This means the method might wrongly mark some labeled images as mislabeled.

## Q4
Label smoothing with a factor of 0.2 performed better than the noisy‑label baseline. Its noisy validation accuracy was 55.76 percent compared with 49.08 percent for the noisy‑label baseline. Label smoothing prevents the model from becoming too confident, in a label. This helps reduce the effect of labels during training and improves classification performance.

## Q5
No the ranking did not change. Label smoothing performed better than the baseline on both synthetic noise. For noise label smoothing achieved 49.72% validation accuracy compared with 41.10% for the baseline. For noise label smoothing achieved 55.76% compared with 49.08%, for the baseline. This shows that label smoothing helped in both cases even though human labeling mistakes and generated mistakes can have different patterns.