# ML Toolkits - Introduction

**TODO** check validity

AI is becoming increasingly important in Earth observations as most parts of the Earth system are continuously monitored by sensors and AI is able to cope  with both the volume of data and the heterogeneous data characteristics. For instance, satellites monitor the atmosphere, land, and ocean with unprecedented accuracy. In FAIRiCUBE the Jupyter-Lab capabilities have been extended to support the application of machine learning (ML) methods on datacubes.

We provide three Python-based best practice [Jupyter Notebooks](example.md#example-notebooks) based on a generic use case to showcase the implementation of state-of-the-art machine learning libraries in the FAIRiCUBE Hub environment. Each Jupyter Notebook involves a self-contained workflow, markdown cells, comments and plots for user-friendly application and guidance and is based on one of the three well established open source ML libraries respectively:

1. [scikit-learn](https://scikit-learn.org/stable/)<br>
For classical machine learning such as support vector machines, decision trees, regressions or clustering, scikit-learn provides a broad set of features that fulfils many basic requirements.
2. [PyTorch](https://pytorch.org/)<br>
For larger neural networks and support for Deep Learning additional ML toolchains are necessary, for example the python-based ML stack PyTorch. With PyTorch, experienced users are supported. It provides low-level API and allows for flexibility to develop and customize deep learning models. It allows for GPU computation and supports transfer learning, domain adaptation, or diverse methods for fine tuning of models.
3. [TensorFlow/Keras](https://www.tensorflow.org/guide)<br>
Keras provides a high-level API that can be run on the popular execution backend TensorFlow. Due to its simplicity, it fits well to the requirements of those Earth system scientist that do not require to newly develop neuronal network architectures. As PyTorch, TensorFlow is python-based, allows for GPU computation and it supports Deep Learning applications including transfer learning or domain adaptation.

Model tracking is realized through the usage of [TensorBoard](https://www.tensorflow.org/tensorboard) and
[mlflow](https://mlflow.org/). These tools offer science teams an easy-to-use platform allowing to run and scale their Machine Learning workloads in a collaborative environment supporting versioning and sharing of parameters, models, artefacts, results, etc. within the team and potentially external users.
Mlflow supports the MLOps pipelines particularly to log and evaluate experiment runs as well as to store models in a registry​. Persistent mlflow deployments are made available on team level to allow each team member to compare their experiments with those of the other team members and to use the trained models of others.
TensorBoard as another collaborative tool in this MLOPs space is currently evaluated by the science teams and available as part of the TensorFlow conda kernel to individual users within their JupyterLab session.

<p align="center">
  <img src="../../images/mlflow.png" alt="mlflow.png"/>
</p>
<p align = "center">
  <i>Collaborative Experiment Tracking with mlflow</i>
</p>

One may also want to reuse information gained during model training for a
second related task, especially when it comes to a lack of data. A PyTorch
based Jupyter Notebook provides the implementation of
`DeepESDL`[Transfer Learning](https://github.com/deepesdl/ML-Toolkit/blob/master/src/transfer_learning.ipynb). <https://github.com/deepesdl/ML-Toolkit/blob/master/src/transfer_learning.ipynb>

<p align="center">
  <img src="../../images/transfer_learning.png" width="75%" height="75%">
</p>
<p align = "center">
<i>The Basic Concept of Transfer Learning</i>
</p>


## FAIRiCUBE - MLflow
Each Use Case team decides which apps shall be made available. One of these apps is MLflow.<br>
MLflow is an open-source platform for managing the end-to-end machine learning lifecycle. It allows the user to track experiments, package code into reproducible runs, and share and deploy models. <br>
MLflow can be incorporated into Jupyter notebooks or other code and supports multiple programming languages. MLflow provides a comprehensive solution for managing the machine learning lifecycle, from tracking experiments to deploying models. It is widely used in industry and academia and is constantly evolving to support the latest trends and technologies in the field of machine learning. <br>
At a high level, MLflow consists of four main components: tracking, projects, models, and registry. <br>
All components can be accessed via Python code in the FAIRiCUBE Lab.


### MLflow Tracking
The MLflow tracking component (here an example form DeepESDL) allows users to log and track training parameters, code, and output metrics from their machine learning experiments.

![mlflow.png](../../images/mlflow.png)

The tracking component provides an API for Python, R, and other languages, as well as an UI for visualising experiments and comparing different runs. The tracking server can store data in various backends, including a local file system, an Amazon S3 bucket, or a PostgreSQL database.<br>
MLflow Tracking uses the concept of runs, which are executions of some piece of data science code, e.g., training of models. MLflow Tracking supports auto-logging for many classic libraries such as TensorFlow, Scikit-Learn, Spark, or Pytorch, but manual logging is available in other cases. Runs can be stored as local files, on a remote server, or into an SQLAlchemy compatible database. The tracking UI allows to directly visualise tracked metrics and search for the best components.


### MLflow Projects
The MLflow projects component provides a standard format for packaging and distributing machine learning code, including dependencies, in a reproducible way. Projects can be run locally or on a cluster, and MLflow can manage the environment and dependencies for each run. <br>
In addition, the Projects component includes an API and command-line tools for running projects, making it possible to chain together projects into workflows. In the MLproject file it is possible to define the software environment and entry points with parameters to define workflow.


### MLflow Models
The models component allows users to easily package models in a standard format for deployment. Models can be exported in multiple formats, including TensorFlow, PyTorch, and ONNX, and can be deployed using a variety of tools, including Docker, Kubernetes, and Amazon SageMaker. <br>
It is also possible to access models with standard ways as REST API or batch inference on Apache Spark. Native flavours allow MLflow models to be treated with corresponding functions without the need to integrate tools with each library. Flavours can be defined in the MLmodel file. Model signatures are defining outputs and inputs needed for deploying models as a REST API.<br>
The Model API allows saving, loading, and logging of the model also as adding different flavours. MLflow also provides an evaluate API to evaluate previously built models on one or more datasets.


### MLflow Model Registry
Finally, the MLflow Model Registry component allows users to store, manage, and deploy models in a central repository. Models can be versioned, and access can be controlled using role-based access control. The Model Registry works both in UI and API versions.
It provides model lineage (which MLflow experiment and run produced the model), model versioning, stage transitions (for example from staging to production), and annotations. Model versioning allows models to be archived and redeployed in the future.


## Overview
1. [Getting Started](ml_getting-started.md)
2. [Example Use Case and Juypter Notebooks](ml_example.md)
3. [Recommendations and Considerations](ml_recommendations.md)

