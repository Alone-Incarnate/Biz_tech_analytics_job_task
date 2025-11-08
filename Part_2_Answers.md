answer - 1. I would use segmentation first because it can clearly show if a label is missing or not.If that is too slow or not accurate, i would try detection only for the label area.And as a backup, I would crop the product and run a small classifier to check if the label exists.

answer - 2. I will check if the new images look different in lighting, angle, or background because then only a model can give poor result and if possible i will try to reduce the training image as some time more image just over train the model and will use augumentation to improve accuracy because sometimes different lighting can cause low accuracy.

answer - 3. Accuracy is not the right metric here. I would look at recall and false negatives since missing a defect is more serious. It is fine to have a few false alarms as long as no bad product gets through.

answer -4 . I will keep slightly blurry or partial images if they represent real situations.But if they’re too unclear then i will remove them.Some imperfect data helps the model adapt the real world situation, but too much can cause confusion.
