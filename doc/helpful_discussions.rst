===================
Helpful Discussions
===================

Adding user/item features makes my model perform worse than without features
============================================================================
That's not unusual and might have different reasons. For one, make sure you 
don't drop per-user/item features, see :doc:`LightFM<lightfm>`. If that
doesn't help, your features might be simply uninformative and worsen the 
signal to noise ratio. You can experiment with different features and try
discretization strategies for continous features. More strategies and ideas
can be found here:

- https://github.com/lyst/lightfm/issues/551
- https://github.com/lyst/lightfm/issues/486
- https://github.com/lyst/lightfm/issues/176
- https://github.com/lyst/lightfm/issues/430

My model is recommending mostly the same very popular items to all users
========================================================================
You might consider applying inverse propensity weights to your features. 
See these issues for more information:

- https://github.com/lyst/lightfm/issues/176
- https://github.com/lyst/lightfm/issues/395

Iterative Training / New Users / Fold-In
========================================
- https://github.com/lyst/lightfm/issues/194

Hyperparameter Optimization
===========================
-https://gist.github.com/maciejkula/29aaf2db2efee5775a7f14dc387f0c0f

Cold-Start
==========
- https://stackoverflow.com/questions/46924119/lightfm-handling-user-and-item-cold-start
- https://github.com/lyst/lightfm/issues/371

Time Context Information
========================
- https://github.com/lyst/lightfm/issues/237

Memory Limits / Memmapped arrays 
================================
- https://github.com/lyst/lightfm/issues/389

Predict for all users / Batch Prediction / BLAS Predict
=======================================================
- https://github.com/lyst/lightfm/issues/427
- https://github.com/inpefess/lightfm/blob/predict_comparison/examples/batch_predict/predicting_with_matrix_multiplication.ipynb

Large Matrices / Helper Tools for Data Prep
===========================================
- https://github.com/lyst/lightfm/issues/258
- https://github.com/DomainGroupOSS/ml-recsys-tools/blob/df866704b1ab3ad05dbe40ebd4b2d92d071f8eab/ml_recsys_tools/data_handlers/interactions_with_features.py#L154


Short-Lived Items?
==================
- https://github.com/lyst/lightfm/issues/449

