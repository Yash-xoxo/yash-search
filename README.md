<!-- # Personal Portfolio ⚡️ 
> A clean, beautiful, responsive portfolio template for Software Developers!!!

[search-page](https://yash-xoxo.github.io/yash-search/)

![GitHub stars](https://img.shields.io/github/stars/yash-xoxo/yash-xoxo.github.io) 
![GitHub forks](https://img.shields.io/github/forks/yash-xoxo/yash-xoxo.github.io)
[![Maintenance](https://img.shields.io/badge/maintained-yes-green.svg)](https://github.com/yash-xoxo/yash-xoxo.github.io/commits/master)
[![Website shields.io](https://img.shields.io/badge/website-up-yellow)](http://yash-xoxo.github.io/)
[![Ask Me Anything !](https://img.shields.io/badge/ask%20me-linkedin-1abc9c.svg)](https://www.linkedin.com/in/yash-gupta-4285b8312/)
[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

### Website Preview
<p align="center"> 
  <kbd>
    <a href="https://yash.github.io" target="_blank"><img src="examples/preview.gif">
  </a>
  </kbd>
</p>

:star: Star me on GitHub — it helps!


PAY - bc1qfqqqerfcyz6y088hgwk63gctk5ynvdfcfmefv2


## Features 📋
⚡️ Fully Responsive\
⚡️ Valid HTML5 & CSS3\
⚡️ Typing animation using `Typed.js`\
⚡️ Easy to modify

## Sections 📚
✔️ About me\
✔️ Experience\
✔️ Projects \
✔️ Skills \
✔️ Education\
✔️ Contact Info\
✔️ Resume

To view a live example, **[click here](https://yash-xoxo.github.io/yash-portfolio/)**

## Tools Used 🛠️
* [<b>GitHub Pages</b>](https://create-react-app.dev/docs/deployment/#github-pages) - To host my static website (HTML, CSS, JS).
* [<b>Materialize</b>](https://materializecss.com/) - A CSS framework to get Google's Material Design components.
* [<b>Typed.js</b>](https://mattboldt.com/demos/typed-js/) - JavaScript Library

## Contributing 💡
#### Step 1

- **Option 1**
    - 🍴 Fork this repo!

- **Option 2**
    - 👯 Clone this repo to your local machine.


#### Step 2

- **Build your code** 🔨🔨🔨

#### Step 3

- 🔃 Create a new pull request.

## License 📄
This project is licensed under the MIT License - see the [LICENSE.md](./LICENSE) file for details.
# yash-portfolio
# yash-portfolio
-->

# Interview Prep — Resume Walkthrough
**For: Yash Gupta | DevOps & Cloud Developer**

This guide explains every technology, certification, and project on your resume — what it is, and a ready-to-use line for when the interviewer asks "tell me about this."

---

## PART 1: Core DevOps Tools

### Docker
**What it is:** Packages an application + all its dependencies into a single portable "container" so it runs identically on any machine.
**Say:** "I used Docker to containerize applications so they'd run consistently across dev, test, and simulated production environments — eliminates the 'works on my machine' problem."
**Likely follow-up:** *Difference between a container and a VM?* → A VM virtualizes hardware and runs a full OS; a container shares the host OS kernel and only packages the app + libraries, so it's lighter and starts in seconds, not minutes.

### Kubernetes (K8s)
**What it is:** An orchestration platform that manages many containers across many machines — handles scaling, restarts, load balancing, and self-healing automatically.
**Say:** "I used Kubernetes to deploy and manage containerized workloads, including setting up autoscaling so the cluster could handle variable traffic without manual intervention" (ties directly to your Auto-Scaling project).
**Likely follow-up:** *What's a Pod vs a Deployment vs a Service?* → Pod = smallest deployable unit (one or more containers); Deployment = manages a set of identical Pods and handles rollouts/rollbacks; Service = stable network endpoint that routes traffic to the right Pods even as they're replaced.

### Jenkins
**What it is:** An automation server used to build CI/CD pipelines — automatically tests and deploys code whenever it changes.
**Say:** "I built Jenkins pipelines that trigger on a Git commit, run automated tests, then build and push a Docker image — so deployment becomes a repeatable, hands-off process instead of a manual one."
**Likely follow-up:** *Declarative vs Scripted pipeline?* → Declarative uses a structured, easier-to-read syntax (`pipeline {}` blocks) ideal for most CI/CD; Scripted is raw Groovy code, more flexible but harder to maintain.

### Terraform
**What it is:** An Infrastructure-as-Code (IaC) tool — you describe the infrastructure you want (servers, networks) in code, and it creates/manages it for you.
**Say:** "I used Terraform to provision infrastructure automatically instead of clicking through the AWS console manually — this cuts setup time and means infrastructure changes are version-controlled, just like application code."
**Likely follow-up:** *What's a Terraform state file?* → It tracks what infrastructure Terraform has already created, so it knows what to change/add/destroy on the next run instead of recreating everything from scratch.

### Ansible
**What it is:** A configuration management tool — automates installing software, applying settings, and configuring servers, using simple YAML "playbooks."
**Say:** "Where Terraform provisions the infrastructure, Ansible is what I'd use to configure it afterward — installing packages, setting up users, applying consistent configuration across multiple servers without SSHing into each one manually."
**Likely follow-up:** *Ansible vs Terraform — why use both?* → Terraform is best at creating/destroying infra (servers, networks); Ansible is best at configuring what's already running (software, files, services). They're complementary, not competing.

### Git / GitHub Actions
**What it is:** Git = version control for code. GitHub Actions = CI/CD automation built directly into GitHub (an alternative/complement to Jenkins).
**Say:** "I use Git for version control on all my projects, and GitHub Actions for lightweight CI/CD directly inside GitHub — useful when you don't want to run and maintain a separate Jenkins server."

---

## PART 2: Cloud Platforms — AWS

| Service | What it does | One-liner to use |
|---|---|---|
| **EC2** | Virtual servers in the cloud | "EC2 gave me on-demand compute to host applications without owning physical hardware." |
| **S3** | Object storage (files, backups, static sites) | "I used S3 for storing artifacts/static assets — durable, cheap, and accessible from anywhere." |
| **IAM** | Identity & Access Management — controls *who* can do *what* | "IAM is how I enforced least-privilege access — giving services and users only the permissions they actually need." |
| **VPC** | Virtual Private Cloud — your own isolated network inside AWS | "VPC let me control networking — subnets, routing, and security groups — to isolate and secure resources." |
| **CloudWatch** | AWS's monitoring & logging service | "CloudWatch gave visibility into resource health and triggered alerts on abnormal metrics." |

**Likely follow-up:** *What's the difference between a Security Group and a NACL?* → Security Groups are stateful and attached to instances (allow rules only); NACLs are stateless and attached to subnets (can allow AND deny).

---

## PART 3: Monitoring & Observability

### Prometheus
**What it is:** An open-source monitoring system that "scrapes" (pulls) metrics from your systems at regular intervals and stores them as time-series data.
**Say:** "I set up Prometheus to continuously collect system and application metrics — CPU, memory, request rates — so issues could be caught before they became outages."

### Grafana
**What it is:** A visualization dashboard tool — usually paired with Prometheus to turn raw metrics into readable graphs and alerts.
**Say:** "Grafana is what turned Prometheus's raw metrics into dashboards the team could actually look at — and I configured alerts for thresholds like high CPU or memory usage."

### Node Exporter
**What it is:** A small agent that runs on a server and exposes hardware/OS-level metrics (CPU, disk, memory, network) in a format Prometheus can scrape.
**Say:** "Node Exporter is what fed host-level metrics into Prometheus — without it, Prometheus only sees application metrics, not the underlying server health."

---

## PART 4: Infrastructure & Automation Concepts

- **CI/CD (Continuous Integration / Continuous Deployment):** CI = automatically testing every code change; CD = automatically deploying changes that pass. Together they shrink the gap between writing code and it being live.
- **IaC (Infrastructure as Code):** Treating infrastructure setup (servers, networks) as code — version-controlled, repeatable, reviewable — instead of manual console clicks.
- **Containerization:** Packaging an app with everything it needs to run, so it behaves the same anywhere (laptop, test server, production cloud).

---

## PART 5: Operating Systems — Linux (Arch, Ubuntu, RHEL, Fedora)

**Why list multiple distros:** Shows you're not just comfortable in one Linux flavor — you understand differences in package managers and philosophy.
**Say:** "I'm comfortable across distros — Ubuntu/Debian-based systems use `apt`, RHEL/Fedora use `dnf`/`yum`, and Arch uses `pacman`. RHEL specifically is what most enterprise environments run, which is part of why I pursued the RHCSA certification."

---

## PART 6: Programming & Scripting

- **Python:** General-purpose scripting and automation language — used for tooling, simple APIs (Flask), and integrating AI APIs (as in your n8n project).
- **Bash:** Shell scripting for automating command-line tasks on Linux — cron jobs, deployment scripts, log parsing.
- **Flask:** A lightweight Python web framework — good for building small APIs/dashboards quickly (you used this in your Automation Project hub).

---

## PART 7: Certifications — What Each One Proves

| Certificate | What it signals to an interviewer |
|---|---|
| **AWS Cloud Quest: Cloud Practitioner** | Foundational AWS knowledge — core services, billing, shared responsibility model |
| **AWS Cloud Quest: Generative AI Practitioner** | Awareness of AWS's AI/ML services (Bedrock, SageMaker concepts) |
| **LFS170 – Blockchain: Understanding Its Uses and Implications** | Conceptual understanding of decentralized systems (not a core DevOps skill, but shows breadth — be ready to explain *why* you took it briefly) |
| **LFS158 – Kubernetes for Beginners (JP)** | Structured, vendor-neutral K8s fundamentals from the Linux Foundation itself (the org that stewards Kubernetes) |
| **RHCSA (EX200)** | The big one for Linux credibility — a *hands-on, performance-based* exam (not multiple choice), proving you can actually administer a Red Hat system: users, permissions, storage, networking, services |
| **PostgreSQL Bootcamp** | Practical relational database skills — useful since most apps you deploy will need a DB tier |
| **AWS Cloud + AI Workshop / JASBAA 4.0** | Practical/workshop exposure — fine to mention briefly as supplementary, not your headline credentials |

**Tip:** If asked "which certification are you most proud of," lead with **RHCSA** — it's the most rigorous (hands-on lab exam, not a quiz) and most directly relevant to a DevOps role.

---

## PART 8: Work Experience — DevOps Engineer Intern, LinuxWorld Informatics (Jun–Aug 2025)

Be ready to turn each resume bullet into a 20-30 second story (Situation → Action → Result):

1. **"Built and managed containerized environments using Docker and Kubernetes to simulate production workloads"**
 → *Say:* "I containerized sample applications with Docker and deployed them on Kubernetes, simulating how a real production environment would handle multiple services running together."

2. **"Designed CI/CD pipelines using Jenkins"**
 → *Say:* "I set up Jenkins pipelines so that every code change automatically triggered a build, ran tests, and deployed — removing manual steps from the release process."

3. **"Automated infrastructure provisioning using Terraform"**
 → *Say:* "Instead of manually creating servers each time, I wrote Terraform configs so infrastructure could be spun up consistently and quickly, and torn down just as easily."

4. **"Implemented monitoring and alerting using Prometheus and Grafana"**
 → *Say:* "I set up the monitoring stack so the team could see system health in real time and get alerted before small issues became outages."

5. **"Maintained Linux-based servers and resolved real-time infrastructure issues under simulated production traffic"**
 → *Say:* "I handled day-to-day Linux server administration and troubleshot issues while traffic simulations were running, which gave me hands-on debugging experience under pressure."

6. **"Collaborated with DevOps mentors on scalable deployment strategies"**
 → *Say:* "I worked closely with my mentors to review deployment approaches and incorporate feedback — a lot of what I learned about doing things 'the production-grade way' came from that back-and-forth."

**Capstone mention:** Your **Automation Project** (Docker, K8s, AWS, Terraform, Ansible, Jenkins + a Streamlit dashboard) was your way of tying every tool together into one working system — good to mention as "the project where everything from the internship came together in one place."

---

## PART 9: Projects — Deep Dive

For each project below: **Elevator pitch** (use this if asked "walk me through this project") → **How it works** → **Questions to expect**.

### 1. Proxmox Virtualization Infrastructure (Type-1 Hypervisor)
- **Stack:** Proxmox VE, KVM/QEMU, LXC, Debian, ZFS
- **Elevator pitch:** "I built a home virtualization lab using Proxmox — a Type-1 hypervisor — to run multiple isolated VMs and containers for testing DevOps tools without needing separate physical machines."
- **How it works:** Proxmox runs directly on hardware (Type-1 = no host OS in between, unlike VirtualBox which is Type-2). KVM/QEMU provide full VMs; LXC provides lightweight Linux containers sharing the kernel. ZFS is the filesystem, chosen for snapshots and data integrity.
- **Expect:** *"Why Proxmox over plain VirtualBox?"* → Proxmox is built for production-style multi-VM management with clustering, live migration, and a web UI — VirtualBox is single-machine, desktop-oriented. *"Why ZFS?"* → Built-in snapshotting and protection against data corruption, useful for quickly reverting a broken VM.

### 2. n8n-Driven AI Workflow Engine
- **Stack:** n8n, Gemini API, Telegram/Discord Bots, Docker, RSS Frameworks
- **Elevator pitch:** "I built an automated pipeline that pulls DevOps/cloud news via RSS every 45 minutes, summarizes it using the Gemini API, and publishes the summary to Telegram and Discord — so I get curated, digestible updates without manually checking ten sites a day."
- **How it works:** n8n is a no-code/low-code workflow automation tool (like Zapier, but self-hostable) — it's the "orchestrator" connecting the RSS trigger → the AI summarization step → the chatbot publishing step. The whole thing runs in Docker for portability.
- **Expect:** *"Why n8n instead of writing it all in Python?"* → Faster to build and visually easier to debug a multi-step pipeline; also easy to swap one step (e.g., a different AI model or a new publishing channel) without rewriting code. *"What happens if the Gemini API fails?"* → Good moment to mention error handling/retry logic if you implemented it, or to honestly say "currently it would skip that cycle — a good next improvement would be a retry-with-backoff step."

### 3. Containerized Full-Stack Travel Platform
- **Stack:** React, Node.js, Express, MongoDB, Docker Compose
- **Elevator pitch:** "I built a full travel booking platform — React frontend, Node/Express backend, MongoDB for data — with each piece running in its own Docker container, wired together with Docker Compose."
- **How it works:** Docker Compose defines and runs multiple containers (frontend, backend, database) as one unit with a single command, including the networking between them. Auth workflows secure login/booking; CRUD = Create/Read/Update/Delete operations for bookings.
- **Expect:** *"Why microservices/containers for this instead of one monolith?"* → Service isolation — if the frontend needs an update, you don't have to touch or redeploy the backend or DB; each piece scales and fails independently. *"How did you handle auth?"* → Be ready to describe whatever you actually used (JWT tokens is the common answer for a MERN-style stack — confirm what you implemented before the interview).

### 4. Kubernetes Auto-Scaling Web Cluster
- **Stack:** Kubernetes (HPA), Minikube, Docker, Apache HTTPD
- **Elevator pitch:** "I built a self-healing, load-adaptive web cluster on Kubernetes using Horizontal Pod Autoscaling — when CPU load increased, the cluster automatically spun up more replica pods to handle it, and scaled back down when load dropped."
- **How it works:** HPA (Horizontal Pod Autoscaler) watches a metric (usually CPU%) and adjusts the number of running Pod replicas automatically. Minikube = a local single-node Kubernetes cluster for testing without needing cloud infrastructure. NodePort exposes the service on a static port so it's reachable for traffic testing.
- **Expect:** *"How does HPA actually decide when to scale?"* → It compares current average resource usage across pods against a target threshold you set (e.g., 50% CPU) and calculates how many replicas are needed to bring usage back to target. *"NodePort vs LoadBalancer vs ClusterIP?"* → ClusterIP = internal-only access; NodePort = exposes a port on every node (good for local/test); LoadBalancer = provisions an actual external load balancer (cloud-only, production use).

### 5. CI/CD Pipeline for Python Microservices
- **Stack:** Jenkins, GitHub, Docker, Pytest
- **Elevator pitch:** "I built a fully automated pipeline for Python microservices — a GitHub commit triggers Jenkins, which runs Pytest for automated testing, then builds a Docker image and pushes/deploys it — simulating a production-grade release process."
- **How it works:** Webhook from GitHub notifies Jenkins of a new commit → Jenkins job checks out code → runs Pytest suite → if tests pass, builds a Docker image → pushes it to a registry → deploys.
- **Expect:** *"What happens if tests fail?"* → The pipeline should stop before the build/deploy stage — this is the whole point of CI, catching bugs before they ship. *"How is this different from project #4's pipeline?"* → This one is the CI/CD pipeline itself (build/test/deploy automation); project #4 is about what happens *after* deployment (scaling the running service).

### 6. Offline AI Model Ecosystem
- **Stack:** Ollama, Hugging Face, Open WebUI, DeepSeek, LLaMA 3.1, Gemma
- **Elevator pitch:** "I set up a fully local AI environment that runs large language models and vision models on my own hardware with no internet dependency — useful for privacy, cost control, and offline experimentation."
- **How it works:** Ollama is a tool for running open-source LLMs locally with simple commands; Open WebUI gives it a ChatGPT-style interface; Hugging Face is where many of the models (DeepSeek, LLaMA 3.1, Gemma) are sourced from. "Hardware-accelerated" means using your GPU (if available) instead of CPU for much faster inference.
- **Expect:** *"Why run models locally instead of just using an API like OpenAI's?"* → No per-token cost, no data leaving your machine (privacy), and it works without internet — tradeoff is you need decent hardware and the models are generally smaller/less capable than the largest cloud models. *"What hardware did you run this on?"* → Have your actual GPU/CPU specs ready.

---

## PART 10: Gaps to Be Ready For

Your resume is strong on the foundational toolchain (Docker, K8s, Jenkins, Terraform, Ansible, Prometheus/Grafana). A DevOps interviewer at a company already running Kubernetes in production may probe slightly past what's listed here — it's worth having a short, honest answer ready rather than being caught off guard:

- **Helm / ArgoCD / GitOps:** If asked, you can say: "I haven't used Helm or ArgoCD directly yet, but I understand the concept — Helm packages Kubernetes manifests into reusable templates ('charts'), and ArgoCD/GitOps means your Git repo becomes the single source of truth for what's deployed, with the cluster auto-syncing to match it. It's next on my list to get hands-on with."
- **Managed Kubernetes (EKS/GKE) vs. self-managed/Minikube:** Your hands-on work is on Minikube — be upfront: "My hands-on K8s work has been on Minikube for learning and prototyping; I haven't yet run a workload on EKS, but the core concepts (Pods, Deployments, Services, HPA) transfer directly — the main difference is AWS managing the control plane for you."

Naming the gap confidently and explaining what you *do* understand conceptually lands much better than dancing around it.

---

## PART 11: Likely General Questions

- "Walk me through your resume" → Use the internship summary (Part 8) then pick 1-2 favorite projects (Part 9).
- "Which project are you most proud of and why?" → Pick one where you can speak to a real technical decision you made (autoscaling thresholds, why Docker Compose, why ZFS, etc.) — specificity beats breadth.
- "What was the hardest bug you debugged?" → Prepare one real story (any project) with: what broke, how you diagnosed it (logs? `kubectl describe`? Jenkins console output?), and the fix.
- "How do you decide what to monitor / alert on?" → Mention chasing actionable signals (CPU/memory/error rate thresholds) over noisy alerts.
