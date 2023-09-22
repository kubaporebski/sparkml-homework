# Spark Machine Learning Homework

## Screenshots from following the notebook steps

* Cloudpickle installation

![](docs/install_cloudpickle.png)

* Importing data into DBFS and preparing it was done correctly. I followed instructions and uploaded data via Databricks UI.  
* So this time, there was no need for another Google Cloud bucket, I didn't have to use `terraform`.
* Here you can see the resulting pandas dataset:

![](docs/pandas_data_ready.png)

* How's quality of wine distributed? Histogram shows it:

![](docs/plot_quality.png)

* In the dataset independent variables are variables used to predict a dependent variable. So, we use `fixed_acidity`, `citric_acid`, `density`, `pH`, `alcohol`, etc. 
to predict dependent variable with name `quality`.
* Independent variables vs. dependent variable, visualized in a series of plots:

![](docs/lots_of_plots.png)
* 
* Let's train dataset and run machine learning. We're using `MLFlow` framework to do it.
* After ML training, we know what features have most impact on the wine quality. Let's check:

![](docs/feature_importances.png)

* After training, we can register a resulting model.

![](docs/model_registered.png)

* We can promote this model to a production stage.

![](docs/model_production_stage.png)

* What is AUC (area under curve) of that registered model?

![](docs/registered_production_model_auc.png)

* Now, onto the advanced features of Machine Learning. Let's try a hyperparameter sweep.

![](docs/hyperparameter_sweep_in_a_run.png)

* We can go into MLFlow dedicated page and see on the parallel coordinates plots how was a run:

![](docs/parallel_coords_plot.png)

* Let's promote the best performing model to a production stage, and archive an old version of previous one.

![](docs/new_version_of_model_promoted.png)

* We can serve this model - the newest version of it - as well.

![](docs/model_serving.png)

* And done!
