<p>
  <a href="https://learnsome.tech/courses/kubernetes-course">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset=".github/assets/wordmark-inverse.svg">
      <img src=".github/assets/wordmark.svg" alt="LearnSome.tech" width="260">
    </picture>
  </a>
</p>

# Kubernetes: Production-Grade Container Orchestration

**Zero Downtime Deployments, Ingress, Observability, and Secrets**

8 modules, 44 lessons: The Cluster And Your First Diagnosis; Running And Repairing Workloads; Services And External Traffic; Configuration And Persistent Data; Scheduling And Resource Pressure; Identity And Pod Security; Cluster Operations And Recovery; Packaging, GitOps And Operators. Advanced level, about 2 hours.

This repository holds the labs of the free lessons of the LearnSome.tech course [Kubernetes: Production-Grade Container Orchestration](https://learnsome.tech/courses/kubernetes-course): each lab's starter files, a README with the goal, the steps and the expected output, and `./check`, which tests your work the way the site does.

## Start

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/learnsome-tech/kubernetes-free-labs?quickstart=1)

- **Codespaces:** the badge opens this repository in a dev container with Python 3.14.7, kubeconform 0.8.0 and ansible-core and yamllint, as in the site's lab sandbox.
- **On your machine:**

  ```sh
  git clone https://github.com/learnsome-tech/kubernetes-free-labs.git
  cd kubernetes-free-labs
  ./check m01l01-02
  ```

  You need Python 3 for `./check`, and for the labs themselves Python 3.14.7, kubeconform 0.8.0 and ansible-core and yamllint. Other versions mostly work, but only the sandbox's versions are sure to print what the site prints. VS Code's Dev Containers extension builds the same container as Codespaces (x86-64).

## Doing a lab

1. Open the lesson on LearnSome.tech and the lab folder beside it: `labs/<lesson>/<lab>/`. The lab README has the goal, the steps and the expected output.
2. Work in the lab's `starter/` folder.
3. From the repository root, run `./check <lab>` (for example `./check m01l01-02`), or `./check <lesson>` for all labs of a lesson, or `./check --all`. `./check --list` shows every lab and how it is checked.

`./check` runs your starter the way the site's lab sandbox does: in a scratch copy that is its working directory and `HOME`, with `LANG=C.UTF-8`, `TZ=UTC`, `input.txt` on standard input, 10 seconds and 256 KiB of output per stream. It then compares the output with the site's own rules, so a pass here is a pass on the site.

| Check | What `./check` does | Labs |
| --- | --- | --- |
| Checker | Validates the file with the checker the site uses (hadolint, kubeconform, actionlint, yamllint, `ansible-playbook --syntax-check` or `terraform validate`); passes when it finds no errors. | 3 |
| Read along | Nothing to run here: the site shows the listing read-only, and the lab README says honestly what it needs (Docker, a cluster, a cloud account...). | 19 |

## What is published, and what is not

This is the **free edition**: the labs of the course's free lessons, the ones anyone with a free LearnSome.tech account can watch. Each lab's starter is the code the lesson shows on screen. There are no reference solutions, no Pro lessons' labs or expected outputs, no narration and no quiz or exercise answers.

The labs of the Pro lessons are on [the course page](https://learnsome.tech/courses/kubernetes-course), where LearnSome.tech runs and grades them in its sandbox with a Pro membership. The full labs repository is private and stays private.

## Modules and lessons

### Module 1: The Cluster And Your First Diagnosis

| # | Lesson | Labs | Access |
| --- | --- | --- | --- |
| 1.1 | [From Docker To Desired State](https://learnsome.tech/learn/kubernetes-course/m01l01) | [6 labs](labs/m01l01/) | Free |
| 1.2 | [Control Plane: etcd, API Server, Scheduler, Controllers](https://learnsome.tech/learn/kubernetes-course/m01l02) | [5 labs](labs/m01l02/) | Free |
| 1.3 | [Worker Nodes: kubelet, Runtime, CNI And kube-proxy](https://learnsome.tech/learn/kubernetes-course/m01l03) | [3 labs](labs/m01l03/) | Free |
| 1.4 | [Bootstrap A Local Cluster And Check Your Context](https://learnsome.tech/learn/kubernetes-course/m01l04) | [4 labs](labs/m01l04/) | Free |
| 1.5 | [Namespaces, Labels And Declarative Manifests](https://learnsome.tech/learn/kubernetes-course/m01l05) | [2 labs](labs/m01l05/) | Free |
| 1.6 | [Troubleshooting: describe, Events And A First Smoke Test](https://learnsome.tech/learn/kubernetes-course/m01l06) | [2 labs](labs/m01l06/) | Free |

**Free** lessons are open to anyone with a free LearnSome.tech account. The rest of the course is on [LearnSome.tech](https://learnsome.tech/courses/kubernetes-course) with Pro.

## Licence

- **Code** (starter files, `check` and `.learnsome/`, the dev container and the workflows) is under the [MIT licence](LICENSE).
- **Written text** (the READMEs and lab instructions) is under [CC BY-NC-SA 4.0](LICENSE-text.md): share and adapt it with attribution to LearnSome.tech, not commercially, under the same licence.
- The LearnSome.tech name and logo are not covered by either licence.

## Contributing and security

This repository is generated from the course. Report a broken lab or a content error [as an issue](../../issues/new/choose); see [CONTRIBUTING.md](CONTRIBUTING.md). Security reports go to [SECURITY.md](SECURITY.md).

© 2026 LearnSome.tech
