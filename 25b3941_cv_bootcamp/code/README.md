# CV Selection Bootcamp - CIFAR-10N (Harshita Sinha, 25b3941)

All five tasks are in one notebook, `CV_Bootcamp.ipynb`. To reproduce: open it in Google Colab with a GPU runtime,
upload the provided files, set the paths at the top and use Runtime > Run all.
Seed = 0, epochs per network = 50 (cross-validation runs: 15).

Setup used for every run: ResNet-18 from model.py trained from scratch, SGD (momentum 0.9, nesterov, weight decay 5e-4),
lr 0.05 with cosine schedule, batch size 128, random crop + flip.

- Task 1: section "Task 1" -> t1_clean_ref.csv, t1_noisy_ce.csv (final epoch of each).
- Task 2: section "Task 2" -> t2_dynamics.csv, t2_early_stop.csv (epoch with the best noisy validation accuracy).
- Task 3: section "Task 3" -> t3_noise_scores.csv (3-fold cross validation, best signal: cv_loss).
- Task 4: section "Task 4" -> t4_label_smoothing.csv (label smoothing 0.2).
- Task 5: section "Task 5" -> t5_baseline_synth.csv, t5_best_synth.csv.

Clean labels are used only for the Task 1 reference model and for measuring (confusion matrix, Task 2 curves, my Task 3 check).
