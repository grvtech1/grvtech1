<!-- ════════════════════════════════════════════════════════════════
     GitHub Profile README  →  goes in repo: grvtech1/grvtech1 (README.md)
     ════════════════════════════════════════════════════════════════ -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a2540,100:1a73e8&height=200&section=header&text=Gaurav%20Pal&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=DevOps%20Engineer%20%E2%80%A2%20Cloud-Native%20%E2%80%A2%20CI%2FCD%20%E2%80%A2%20GitOps&descSize=18&descAlignY=60" width="100%"/>

<a href="https://www.linkedin.com/in/gauravpal08"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>&nbsp;
<a href="mailto:gorav.p1@aol.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>&nbsp;
<a href="https://github.com/grvtech1"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>&nbsp;
<img src="https://komarev.com/ghpvc/?username=grvtech1&style=for-the-badge&color=1a73e8&label=PROFILE+VIEWS"/>

<br/><br/>

<img src="https://img.shields.io/badge/%F0%9F%9F%A2%20Open%20to%20Work-DevOps%20%C2%B7%20Cloud%20Engineer%20%C2%B7%20Remote%2FHybrid-2ea043?style=for-the-badge"/>

<br/><br/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3500&pause=900&color=1A73E8&center=true&vCenter=true&width=640&lines=Self-managed+Kubernetes+on+AWS;Terraform+%E2%86%92+GitHub+Actions+%E2%86%92+ArgoCD+GitOps;6+microservices+%C2%B7+containerized+%C2%B7+observable;5.5%2B+yrs+IT+%C2%B7+2.5%2B+yrs+DevOps" alt="Typing SVG" />

</div>

---

## 🧑‍💻 About Me

```hcl
resource "devops_engineer" "gaurav_pal" {
  role       = "DevOps Engineer"
  location   = "Noida, India  (open to Remote / Hybrid)"
  experience = "5.5+ yrs IT Ops · 2.5+ yrs DevOps"
  origin     = "Linux & Tech-Support  →  automation  →  cloud-native"

  i_build = [
    "Self-managed Kubernetes (kubeadm + Calico) on AWS EC2",
    "Pull-based GitOps delivery with ArgoCD",
    "Infrastructure as Code with Terraform",
    "CI/CD pipelines — GitHub Actions, Jenkins, Trivy scans",
    "Observability — Prometheus, Grafana, CloudWatch",
  ]

  currently_learning = ["SRE — SLI/SLO/error-budgets", "Advanced K8s patterns", "AWS Solutions Architect"]
  philosophy         = "Automate the toil. Git is the source of truth."
}
```

---

## ⚡ How I Ship

```text
  git push ─▶ GitHub Actions ─▶ test · build · Trivy scan ─▶ GHCR (image:SHA)
                                                                  │ bump tags in deploy/ (commit)
                                                                  ▼
   AWS EC2  ◀── sync ── ArgoCD ◀── watch ── Git (main)   ·   Prometheus ─▶ Grafana / alerts
  (kubeadm K8s)                                              CI never touches the cluster — pull-based GitOps
```

---

## 🚩 Flagship Project — **BillFree TechOps**

> A cloud-native microservices platform built end-to-end and **proven live on AWS**.

[![BillFree TechOps](https://github-readme-stats.vercel.app/api/pin/?username=grvtech1&repo=billfree-techops&theme=react&hide_border=true&bg_color=0a2540&title_color=58a6ff&icon_color=58a6ff)](https://github.com/grvtech1/billfree-techops)

- **6 Node/TypeScript microservices + a React SPA**, fully containerized (multi-stage, non-root images)
- **Self-managed Kubernetes** (kubeadm + Calico CNI) on EC2, provisioned by **Terraform + cloud-init**
- **CI/CD** with GitHub Actions — test matrix → build → **Trivy** scan → push to GHCR
- **Pull-based GitOps** with **ArgoCD** (app-of-apps) — *CI never touches the cluster*
- In-cluster **PostgreSQL** (StatefulSet) + **Redis**, automated DB migrations
- **HPA · PDB · health probes · Ingress**, plus **Prometheus + Grafana** RED-metric dashboards & alerts
- Multi-environment (**dev / staging / prod**) via env-per-folder GitOps overlays

🔗 **[Explore the repo →](https://github.com/grvtech1/billfree-techops)**

---

## ⭐ Featured Project — **VANTA Boutique**

> A cloud-native, **polyglot microservices** e-commerce store — **12 services over gRPC**, extended end-to-end with a brand-new microservice of my own.

[![VANTA Boutique](https://github-readme-stats.vercel.app/api/pin/?username=grvtech1&repo=VANTA-Boutique&theme=react&hide_border=true&bg_color=0a2540&title_color=58a6ff&icon_color=58a6ff)](https://github.com/grvtech1/VANTA-Boutique)

- **12 microservices in 6 languages** (Go · C# · Node.js · Python · Java) talking over **gRPC + Protocol Buffers**
- 🆕 **Built a Reviews microservice** (Go/gRPC) end-to-end — *proto → service → container → K8s → CI/CD* — with a pluggable **in-memory ↔ PostgreSQL** store behind a single `Store` interface
- **Production-hardened**: graceful shutdown (SIGTERM drain), gRPC size/keepalive limits, **DB-driven gRPC health**, `distroless:nonroot` images, dedicated **NetworkPolicy**
- **Kubernetes + Kustomize** (base + overlays + opt-in Postgres component) — runs on **local kind** or **AWS EC2** via **ArgoCD** GitOps
- **CI/CD** with GitHub Actions — `go vet`, **race-detector tests** with a Postgres service container, multi-service Docker builds, **Trivy** scan
- Custom **VANTA** dark-glassmorphism storefront — accessible reviews UI (ARIA) + **schema.org JSON-LD** for rich snippets

🔗 **[Explore the repo →](https://github.com/grvtech1/VANTA-Boutique)**

---

## 🛠️ Tech Stack

#### ☁️ Cloud & Infrastructure
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=FF9900)
![EC2](https://img.shields.io/badge/EC2-FF9900?style=for-the-badge&logo=amazonec2&logoColor=white)
![VPC](https://img.shields.io/badge/VPC-232F3E?style=for-the-badge&logo=amazonvpc&logoColor=white)
![IAM](https://img.shields.io/badge/IAM-DD344C?style=for-the-badge&logo=amazoniam&logoColor=white)
![S3](https://img.shields.io/badge/S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white)
![RDS](https://img.shields.io/badge/RDS-527FFF?style=for-the-badge&logo=amazonrds&logoColor=white)
![CloudWatch](https://img.shields.io/badge/CloudWatch-FF4F8B?style=for-the-badge&logo=amazoncloudwatch&logoColor=white)
![Lambda](https://img.shields.io/badge/Lambda-FF9900?style=for-the-badge&logo=awslambda&logoColor=white)

#### ⚙️ DevOps · IaC · CI/CD
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white)
![ArgoCD](https://img.shields.io/badge/Argo%20CD-EF7B4D?style=for-the-badge&logo=argo&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white)

#### 📈 Observability & Security
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![Trivy](https://img.shields.io/badge/Trivy-1904DA?style=for-the-badge&logo=aqua&logoColor=white)
![Nagios](https://img.shields.io/badge/Nagios-FFA500?style=for-the-badge&logo=nagios&logoColor=white)

#### 🐧 OS · Scripting · Web
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Red Hat](https://img.shields.io/badge/RHEL-EE0000?style=for-the-badge&logo=redhat&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)

---

## 📊 GitHub Stats

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=grvtech1&show_icons=true&theme=react&hide_border=true&bg_color=0a2540&title_color=58a6ff&icon_color=58a6ff&count_private=true" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=grvtech1&layout=compact&theme=react&hide_border=true&bg_color=0a2540&title_color=58a6ff&langs_count=8" />

<br/>

<img src="https://streak-stats.demolab.com?user=grvtech1&theme=react&hide_border=true&background=0a2540&ring=58a6ff&fire=58a6ff&currStreakLabel=58a6ff" height="165" />

<br/><br/>

<img src="https://github-profile-trophy.vercel.app/?username=grvtech1&theme=onedark&no-frame=true&column=7&margin-w=8" />

</div>

---

## 🐍 Contribution Graph

<div align="center">

<img src="https://raw.githubusercontent.com/grvtech1/grvtech1/output/github-contribution-grid-snake-dark.svg" alt="snake animation" />

</div>

---

## 🤝 Let's Connect

<div align="center">

<a href="https://www.linkedin.com/in/gauravpal08"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>&nbsp;
<a href="mailto:gorav.p1@aol.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>&nbsp;
<a href="https://github.com/grvtech1"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/></a>

<br/><br/>

<i>"Infrastructure as code. Delivery as Git. Reliability as a habit."</i>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a73e8,100:0a2540&height=120&section=footer" width="100%"/>

</div>
