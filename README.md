# Hallo! I'm Steve 👋

Software Engineering (Co-op) student at McGill with a minor in Applied AI. I like computer
networking, robotics and 3D modelling, and I'm Software Lead for the McGill Robotics Rover Team.

Most of my time right now goes into a **self-hosted platform I run at home**: a GitOps k3s
cluster plus a handful of Go services that build, trade, investigate and remember things on it.

## 🏠 The homelab

| Repo | What it is | Stack |
|---|---|---|
| [**Homelab**](https://github.com/Blacklotus89898/Homelab) | The umbrella repo. Everything that runs is declared here: ArgoCD app-of-apps, Istio ambient + Gateway API front door, VictoriaMetrics/Grafana, sealed secrets, Backstage, 11 ADRs and a bare-metal rebuild guide | k3s, ArgoCD, Istio, Helm, Kustomize |
| [**Petal**](https://github.com/Blacklotus89898/Petal) 🌸 | Pipeline orchestrator. Schedules, deduplicates and records repo-native YAML pipelines that run as plain Docker containers | Go, SQLite, React |
| [**Tulip**](https://github.com/Blacklotus89898/Tulip) 🌷 | Human-approved trading agent (paper). Rules and Claude propose, a deterministic risk gate disposes, nothing trades without a thumbs-up, and shadow books score every strategy | Go, SQLite, MCP |
| [**Warden**](https://github.com/Blacklotus89898/Warden) | Read-only incident investigator. Collects evidence for every alert and draws a live status map of the cluster | Go, Kubernetes API |
| [**DaVinci**](https://github.com/Blacklotus89898/DaVinci) | Markdown knowledge base with hybrid search, exposed as an MCP server. Runbooks and postmortems the agents read before acting | Go, SQLite FTS5, Ollama |

```mermaid
flowchart LR
  HL[Homelab<br/>GitOps] -->|ArgoCD| K3S[(k3s cluster)]
  PE[Petal<br/>builds] --> K3S
  TU[Tulip<br/>trades] --> K3S
  WA[Warden<br/>investigates] --> K3S
  DV[DaVinci<br/>remembers] -.->|runbooks| WA
```

## 🤖 Robotics and other projects

- [InHouseROS](https://github.com/Blacklotus89898/InHouseROS): my own take on the Robot Operating System, in C++
- [MyROS2](https://github.com/Blacklotus89898/MyROS2) / [MyROS](https://github.com/Blacklotus89898/MyROS): ROS 2 and ROS Noetic robotics (Python, OpenCV, WebRTC)
- [Sodalite](https://github.com/Blacklotus89898/Sodalite): collaborative student dashboard (React, TypeScript, WebRTC)
- [Immovable](https://github.com/Blacklotus89898/Immovable) (Rust, WebAssembly), [GoForSpeed](https://github.com/Blacklotus89898/GoForSpeed) (Go, gRPC)
- [Portfolio](https://blacklotus89898.github.io/Portfolio/)

## 💻 Tech

![Go](https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white) ![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white) ![Argo](https://img.shields.io/badge/argo-%23EF7B4D.svg?style=for-the-badge&logo=argo&logoColor=white) ![Istio](https://img.shields.io/badge/istio-%23466BB0.svg?style=for-the-badge&logo=istio&logoColor=white) ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white) ![Proxmox](https://img.shields.io/badge/proxmox-%23E57000.svg?style=for-the-badge&logo=proxmox&logoColor=white) ![Grafana](https://img.shields.io/badge/grafana-%23F46800.svg?style=for-the-badge&logo=grafana&logoColor=white) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white) ![ROS](https://img.shields.io/badge/ros-%230A0FF9.svg?style=for-the-badge&logo=ros&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) ![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB) ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![Blender](https://img.shields.io/badge/blender-%23F5792A.svg?style=for-the-badge&logo=blender&logoColor=white)

## 📫 Contact

[Website](https://cs.mcgill.ca/~schen183/) · [steve.chen@mail.mcgill.ca](mailto:steve.chen@mail.mcgill.ca)

![](https://github-readme-stats.vercel.app/api?username=Blacklotus89898&theme=vision-friendly-dark&show_icons=true)
![](https://github-readme-stats.vercel.app/api/top-langs/?username=Blacklotus89898&theme=vision-friendly-dark&layout=compact)
