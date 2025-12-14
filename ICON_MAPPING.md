# Custom Icon Mapping

This document shows how custom SVG icons from `assets/icons/` are mapped to technologies across the site.

---

## Available Custom Icons

The following custom SVG icons are available in `assets/icons/`:

| Filename | Technology | Used In |
|----------|-----------|---------|
| `ansible.svg` | Ansible | About, Resume |
| `argo.svg` | ArgoCD | Resume |
| `datadog.svg` | Datadog | About, Resume |
| `digitalocean.svg` | Digital Ocean | Resume |
| `gnubash.svg` | Bash/Shell | About, Resume |
| `go.svg` | Go (Golang) | About, Resume |
| `googlecloud.svg` | Google Cloud Platform (GCP) | About, Resume |
| `grafana.svg` | Grafana | About, Resume |
| `helm.svg` | Helm | Resume |
| `jenkins.svg` | Jenkins | Resume |
| `kubernetes.svg` | Kubernetes | Resume |
| `linux.svg` | Linux | Resume |
| `n8n.svg` | n8n | Resume |
| `owasp.svg` | OWASP ZAP | Resume |
| `prometheus.svg` | Prometheus | About, Resume |
| `python.svg` | Python | About, Resume |
| `sonarqubecloud.svg` | SonarQube | Resume |
| `terraform.svg` | Terraform/Terragrunt | About, Resume |
| `trivy.svg` | Trivy | Resume |

---

## Fallback Icons (Blowfish Built-in)

For technologies without custom SVG files, we use Blowfish's built-in icons:

| Built-in Icon | Technology | Reason |
|---------------|-----------|--------|
| `cloud` | AWS, CloudFormation, AWS CloudWatch | No `aws.svg` available |
| `docker` | Docker | No custom icon available |
| `github` | GitHub, GitHub Actions | Blowfish default |
| `gitlab` | GitLab CI | Blowfish default |
| `search` | ELK Stack | No custom icon available |

---

## Usage in Content

### In About Page (`content/about.md`)

```markdown
{{< keywordList >}}
{{< keyword icon="cloud" >}}AWS{{< /keyword >}}
{{< keyword icon="googlecloud" >}}GCP{{< /keyword >}}
{{< keyword icon="terraform" >}}Terraform{{< /keyword >}}
{{< keyword icon="ansible" >}}Ansible{{< /keyword >}}
{{< keyword icon="go" >}}Go{{< /keyword >}}
{{< keyword icon="python" >}}Python{{< /keyword >}}
{{< keyword icon="gnubash" >}}Bash{{< /keyword >}}
{{< keyword icon="datadog" >}}Datadog{{< /keyword >}}
{{< keyword icon="prometheus" >}}Prometheus{{< /keyword >}}
{{< keyword icon="grafana" >}}Grafana{{< /keyword >}}
{{< /keywordList >}}
```

### In Resume Page (`content/resume.md`)

#### Cloud & Infrastructure
```markdown
{{< keyword icon="cloud" >}}AWS{{< /keyword >}}
{{< keyword icon="googlecloud" >}}GCP{{< /keyword >}}
{{< keyword icon="digitalocean" >}}Digital Ocean{{< /keyword >}}
{{< keyword icon="linux" >}}Linux{{< /keyword >}}
{{< keyword icon="kubernetes" >}}Kubernetes{{< /keyword >}}
{{< keyword icon="docker" >}}Docker{{< /keyword >}}
```

#### IaC & Configuration
```markdown
{{< keyword icon="terraform" >}}Terraform{{< /keyword >}}
{{< keyword icon="ansible" >}}Ansible{{< /keyword >}}
{{< keyword icon="helm" >}}Helm{{< /keyword >}}
```

#### CI/CD & GitOps
```markdown
{{< keyword icon="github" >}}GitHub Actions{{< /keyword >}}
{{< keyword icon="gitlab" >}}GitLab CI{{< /keyword >}}
{{< keyword icon="jenkins" >}}Jenkins{{< /keyword >}}
{{< keyword icon="argo" >}}ArgoCD{{< /keyword >}}
```

#### Security (DevSecOps)
```markdown
{{< keyword icon="sonarqubecloud" >}}SonarQube{{< /keyword >}}
{{< keyword icon="trivy" >}}Trivy{{< /keyword >}}
{{< keyword icon="owasp" >}}OWASP ZAP{{< /keyword >}}
```

#### Observability
```markdown
{{< keyword icon="prometheus" >}}Prometheus{{< /keyword >}}
{{< keyword icon="grafana" >}}Grafana{{< /keyword >}}
{{< keyword icon="datadog" >}}Datadog{{< /keyword >}}
```

#### Programming & Automation
```markdown
{{< keyword icon="python" >}}Python{{< /keyword >}}
{{< keyword icon="go" >}}Go{{< /keyword >}}
{{< keyword icon="gnubash" >}}Bash{{< /keyword >}}
{{< keyword icon="n8n" >}}N8n{{< /keyword >}}
```

---

## How to Add New Custom Icons

1. **Download or create** an SVG file for the technology
2. **Save it** to `assets/icons/` with a descriptive name (e.g., `aws.svg`, `docker.svg`)
3. **Remove the `.svg` extension** when referencing in shortcodes
4. **Update this document** with the new icon mapping

### Example:

If you add `assets/icons/aws.svg`:

```markdown
{{< keyword icon="aws" >}}AWS{{< /keyword >}}
```

---

## Icon Sources

You can find high-quality tech icons from:

- [Simple Icons](https://simpleicons.org/) - Brand SVG icons
- [DevIcon](https://devicon.dev/) - Programming languages and dev tools
- [Skill Icons](https://skillicons.dev/) - Modern tech stack icons
- [Iconify](https://icon-sets.iconify.design/) - Unified icon framework

---

## Notes

- **Icon names are case-sensitive**: Use exact filenames without the `.svg` extension
- **Custom icons override Blowfish icons**: If a custom icon exists with the same name as a Blowfish built-in, the custom one takes precedence
- **SVG optimization**: Keep SVG files small and optimized for web (remove unnecessary metadata)
- **Consistent style**: Try to maintain visual consistency across all custom icons (similar line weights, sizes, etc.)

---

*Last updated: January 2025*