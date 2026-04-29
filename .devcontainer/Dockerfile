# jupyter/scipy-notebook includes: scikit-learn, NumPy, SciPy, matplotlib,
# IPython, Jupyter Notebook, and pandas by default.
FROM quay.io/jupyter/scipy-notebook:latest

USER root
RUN apt-get update && apt-get install -y \
    graphviz \
    && rm -rf /var/lib/apt/lists/*
USER ${NB_UID}

RUN pip install --no-cache-dir graphviz mglearn
