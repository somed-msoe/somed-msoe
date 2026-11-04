<h1 align="center">Delsoro Some</h1>

<p align="center">
  <b>Computer Science @ Milwaukee School of Engineering · Class of May 2027</b><br/>
  Software engineering, machine learning, and secure infrastructure
</p>

<p align="center">
  <a href="https://linkedin.com/in/delsoro-some/"><img src="https://img.shields.io/badge/LinkedIn-delsoro--some-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:somed@msoe.edu"><img src="https://img.shields.io/badge/Email-somed%40msoe.edu-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

---

## About me

- B.S. Computer Science at MSOE, minoring in Cybersecurity
- Working on ML and robotics simulation: deep learning for basketball motion data, and RL-trained robots in NVIDIA Isaac Sim
- I run my own homelab with Docker, Kubernetes (k3s), Ansible, and full monitoring, all managed as code
- Member of the National Society of Black Engineers (NSBE) and the MSOE AI Club

---

## Tech stack

**Languages**

<img src="https://skillicons.dev/icons?i=java,py,cpp,js,html,css,bash,r" alt="Languages"/>

**Web & backend**

<img src="https://skillicons.dev/icons?i=flask,fastapi,react" alt="Web and backend"/> ![SQL](https://img.shields.io/badge/SQL-MSSQL-CC2927?logo=microsoftsqlserver&logoColor=white) ![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?logo=socketdotio&logoColor=white)

**Data science & ML**

<img src="https://skillicons.dev/icons?i=pytorch,sklearn,numpy,pandas" alt="Data science and ML"/>

![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?logo=scipy&logoColor=white) ![NVIDIA Isaac Sim](https://img.shields.io/badge/NVIDIA_Isaac_Sim-76B900?logo=nvidia&logoColor=white)

**Infrastructure, DevOps & security**

<img src="https://skillicons.dev/icons?i=linux,docker,kubernetes,ansible,prometheus,grafana,azure,mongodb" alt="Infrastructure"/> ![Tailscale](https://img.shields.io/badge/Tailscale-242424?logo=tailscale&logoColor=white) ![Gitea Actions](https://img.shields.io/badge/Gitea_Actions-609926?logo=gitea&logoColor=white) ![SLURM](https://img.shields.io/badge/SLURM_HPC-0078D4)

**Tools**

<img src="https://skillicons.dev/icons?i=git,vscode,idea" alt="Tools"/>

---

## Key Projects

### 🏀 Basketball Shot Similarity via Deep Learning
*MSOE Data Science Practicum*

End-to-end similarity search over **~7,000 3D motion-capture basketball shots** (Hawkeye / Second Spectrum data from MongoDB and Azure Blob Storage).

- Trained a **PyTorch convolutional autoencoder** to produce shot embeddings, benchmarked against a Euclidean-distance baseline
- Built explainability tooling (gradient × input attribution, joint-level contribution) to show which body joints drive similarity
- Served top-k retrieval through a **FastAPI** endpoint with a precomputed NPZ cache for sub-second inference
- Built an interactive **React** front end with 3D skeleton rendering and filterable dataset exploration

`PyTorch` `FastAPI` `React` `MongoDB` `Azure`

### 🤖 Autonomous Robot Training Platform: NVIDIA Isaac Sim Digital Twin
*MSOE team research project*

A BIM-to-simulation pipeline that turns Revit building models into USD digital twins, so robots can be trained in a building before it is finished.

- Built reinforcement learning environments (observations, rewards, terminations, curriculum) for NVIDIA Nova Carter and Clearpath Ridgeback robots on autonomous patrol
- Implemented physics-based disaster simulations (fire, flood, buoyancy) and procedural crowds to generate varied anomaly-detection scenarios
- Trained with LiDAR + camera sensors, tracking task completion, path efficiency, and collision frequency
- Ran parallel training on MSOE's **Rosie HPC cluster** (SLURM, NVIDIA T4/H100 GPUs)

`Isaac Sim` `Reinforcement Learning` `Python` `SLURM`

### 🏠 Self-Hosted Homelab Infrastructure
*Personal project*

A single-node Ubuntu Server running ~8 containerized services, managed entirely as code and reachable only over Tailscale (no public port forwards).

- **Infrastructure as Code:** an idempotent Ansible playbook redeploys only changed stacks, validated with dry-run diffs; a self-hosted Gitea Actions runner handles CI and auto-deploy
- **Monitoring:** Uptime Kuma, Prometheus (cAdvisor, node-exporter), provisioned Grafana dashboards, and a healthchecks.io dead-man's switch, with every alert path tested
- **Backups:** nightly encrypted restic backups with an offsite copy, verified by a full restore test
- **Kubernetes:** a version-pinned k3s cluster with Kustomize manifests (health probes, resource limits, pinned images) behind Traefik
- **AI tooling:** a Python **MCP server** that lets AI clients inspect the lab through 7 read-only tools and one gated restart tool

`Docker Compose` `Ansible` `k3s` `Prometheus` `Grafana` `Tailscale` `restic`

### 📦 Audiotec Device Deployment & Imaging Platform
*Software Engineering Internship, Accurate Controls (2025)*

A web-based management system tracking the imaging status and physical location of **2,000+ secure devices** through manufacturing and field deployment.

- **Flask + Socket.IO** interface backed by **MSSQL**, with live progress bars and toast notifications for imaging status
- Searchable, sortable, paginated device table that replaced manual SQL commands for the logistics team
- Reproducible environments through **Ansible and Docker Compose**
- Gathered requirements directly from the logistics manager and iterated on real floor-usage feedback

`Flask` `Socket.IO` `MSSQL` `Ansible` `Docker`

---

## 📊 GitHub stats

<p align="center">
  <img height="170" src="https://streak-stats.demolab.com/?user=somed-msoe&theme=tokyonight&hide_border=true" alt="GitHub streak"/>
</p>

---

<p align="center">
  Open to <b>new-grad software engineering roles</b>, especially backend, ML, and infrastructure.<br/>
  <a href="https://linkedin.com/in/delsoro-some/">Let's connect on LinkedIn</a>
</p>
