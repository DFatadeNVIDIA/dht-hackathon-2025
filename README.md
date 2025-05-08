# DHT Hackathon 2025

This code repository consists of playbooks that can be used to build Digital Human Using [NVIDIA ACE & Tokkio](https://www.nvidia.com/en-us/use-cases/digital-humans/). The playbooks will also cover the process of spinning up the [NVIDIA RAG Blueprint](https://build.nvidia.com/nvidia/build-an-enterprise-rag-pipeline) and connecting the Digital Human to a custom knowledge base. The following notebooks are helpful in the following order:

1. [Tokkio Prerequisites](./notebooks/tokkio_prerequisites.ipynb)
2. [Deploying a TURN Server](./notebooks/deploy_turn_server.ipynb)
3. [Deploying the Tokkio Application (Digital Human Pipeline)](./notebooks/tokkio_app_deploy.ipynb)
4. [Deploying the NVIDIA RAG Blueprint](./notebooks/deploy_nvidia_rag.ipynb)
5. [Customizing Tokkio - Connecting the Avatar to a RAG pipeline](./notebooks/customizing_tokkio.ipynb)

The following prerequisites are expected to be made in order to run through this playbook:

- Ubuntu 22.04 Operating system
- Passwordless sudo access
- Storage requirements:
    - 300GB space on /opt
    - 400GB on /var/lib/containerd
- Required GPU devices for this reference workflow:
    - 2xL40S GPUs
    - 2xL4 GPUs
    - 2xT4 GPUs

**Note**: If Using The Brev Launchable, you'll be provided a 4xL40S GPU instance to enabled multiple concurrent streams when interacting with the avatar (3+). However, for minimal deployments that don't require support for concurrent streams, 2x GPUs are sufficient.

