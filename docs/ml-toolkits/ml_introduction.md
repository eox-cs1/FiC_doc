# ML Toolkits Introduction

AI is becoming increasingly important in Earth observations as most parts of the Earth system are continuously monitored by sensors and AI is able to cope  with both the volume of data and the heterogeneous data characteristics. For instance, satellites monitor the atmosphere, land, and ocean with unprecedented accuracy. In FAIRiCUBE the JupyterLab capabilities have been extended to support the application of machine learning (ML) methods on datacubes.

We provide three Python-based best practice Jupyter Notebooks (Credit: DeepESDL) based on a generic use case to showcase the implementation of state-of-the-art machine learning libraries in the FAIRiCUBE Hub environment. Each Jupyter Notebook involves a self-contained workflow, markdown cells, comments and plots for user-friendly application and guidance and is based on one of the three well established open source ML libraries respectively:

1. [scikit-learn](https://scikit-learn.org/stable/)<br>
For classical machine learning such as support vector machines, decision trees, regressions or clustering, scikit-learn provides a broad set of features that fulfills many basic requirements.
2. [PyTorch](https://pytorch.org/)<br>
For larger neural networks and support for Deep Learning additional ML toolchains are necessary, for example the python-based ML stack PyTorch. With PyTorch, experienced users are supported. It provides low-level API and allows for flexibility to develop and customize deep learning models. It allows for GPU computation and supports transfer learning, domain adaptation, or diverse methods for fine tuning of models.
3. [TensorFlow/Keras](https://www.tensorflow.org/guide)<br>
Keras provides a high-level API that can be run on the popular execution backend TensorFlow. Due to its simplicity, it fits well to the requirements of those Earth system scientist that do not require to newly develop neuronal network architectures. As PyTorch, TensorFlow is python-based, allows for GPU computation and it supports Deep Learning applications including transfer learning or domain adaptation.

Model tracking is realized through the usage of [TensorBoard](https://www.tensorflow.org/tensorboard) or
[MLflow](https://mlflow.org/). These tools offer science teams an easy-to-use platform allowing to run and scale their Machine Learning workloads in a collaborative environment supporting versioning and sharing of parameters, models, artefacts, results, etc. within the team and potentially external users.

# Overview

* [ML-Toolkits Getting Started](ml_getting-started.md)
* [MLflow Introduction](mlflow_introduction.md)
* [ML Toolkit Examples](ml_examples.md)
* TensorFlow Introduction (work in progress)
* TensorFlow Getting Started (work in progress)
* TensorFlow Examples (work in progress)
* PytTorch Introduction (work in progress)
* PytTorch Getting Started (work in progress)
* PytTorch Examples (work in progress)
* scikit-learn Introduction  (work in progress)
* scikit-learn Getting Started (work in progress)
* scikit-learn Examples (work in progress)
<!--* [ML Toolkit Examples](ml_examples.md)
* [TensorFlow Introduction](tf_introduction.md)
* [TensorFlow Getting Started](tf_getting-started.md)
* [TensorFlow Examples](tf_examples.md)-->
<!-- * [Recommendations and Considerations](mlflow_recommendations.md)-->


