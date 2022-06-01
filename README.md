# mlops-pytorch-mlflow-triton

This is a quick example in which you will:
- Train Image classification model based on FashionMNIST dataset using PyTorch framework in Jupyter
- Store the resulting model in MLFlow model registry in ONNX format
- Deploy the model from MLFlow to Triton server

Mentioned above solutions are glued and deployed using Neu.ro MLOps platform. 


## Quick Start

1. Clone guide, install Neu.ro CLI:
    ```shell
    git clone <this repo> && cd <cloned repo directory>
    pipx install neuro-all
    neuro login
    ```

2. Upload the guide notebook and start MLFlow, Triton and Jupyter servers.
    ```shell
    neuro-flow upload ALL
    neuro-flow run mlflow_server
    neuro-flow run triton_server
    neuro-flow run jupyter
    ```

3. Follow the [quickstart_tutorial.ipynb](/notebooks/quickstart_tutorial.ipynb) guide in the oppened Jupyter instance.

    _Note: this guide is based on [PyTorch Quickstart guide](https://pytorch.org/tutorials/beginner/basics/quickstart_tutorial.html)._

4. Cleanup:
    ```shell
    neuro-flow kill ALL
    neuro-flow clean ALL
    ```

See [Help.md](HELP.md) for the detailed Neuro Project Template Reference.
