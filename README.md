# Townsville

Townsville is my self-hosted, three-node Kubernetes homelab running k3s on openSUSE MicroOS, managed declaratively using **Flux CD** and GitOps principles.

This repo serves as the true north for the cluster's Kubernetes configuration, infrastructure, and application deployments. The goal with creating Townsville is for me to learn Kubernetes, GitOps, and other DevOps principles. All while getting to host my other projects and tools myself.

And of course, I had to use fun naming conventions ;)

## Overview

Townsville is still currently a W.I.P.

Townsville is a bare-metal Kubernetes cluster consisting of three nodes running openSUSE MicroOS. Each node participates in the Kubernetes control plane, providing high availability in the event of a node failure through embedded etcd and a shared virtual IP (VIP) address.

Cluster resources and applications are managed using Flux CD, which continuously reconciles the running cluster against the config stored in this repo.

![Diagram](/static/img/Diagram.svg)