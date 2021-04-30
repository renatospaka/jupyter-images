FROM continuumio/anaconda3

## update container
RUN apt-get update && \
    apt-get upgrade -y

WORKDIR /opt/conda/bin

EXPOSE 8888

## update conda 
RUN conda update -n base -c defaults conda -y

## create custom environment & initialize shell
RUN conda create -n dev_env -y  \
    && conda init bash

## Make RUN commands use the new environment:
SHELL ["conda", "run", "-n", "dev_env", "/bin/bash", "-c"]

## prepare environment
RUN mkdir /opt/notebooks

## prepare to install Jupyter
RUN conda install jupyter -y

## launch Jupyter
CMD [ "jupyter", "notebook", "--notebook-dir", "/opt/notebooks", "--ip", "*", "--port", "8888", "--no-browser", "--allow-root" ]
