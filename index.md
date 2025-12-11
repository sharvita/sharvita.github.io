---
layout: null
permalink: /
---
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>{{ site.title }}</title>
    <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@700&family=Antic&family=Montserrat:wght@600,700&family=Inter:wght@400,600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="/styles.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
</head>
<body>

    <header class="site-header">
      <div class="container">
        <a href="/" class="site-title">{{ site.author.name | split: ' ' | first }}</a>
        <nav class="site-nav">
          <a href="/about/">ABOUT</a>
          <a href="#projects-section">PROJECTS</a>
          <a href="{{ site.header.actions | where: 'label', 'View Resume (PDF)' | first | relative_url }}" target="_blank">RESUME</a>
          <a href="mailto:{{ site.header.actions | where: 'label', 'Get In Touch' | first | url | replace: 'mailto:', '' }}">CONTACT</a>
        </nav>
      </div>
    </header>

    <div class="hero-wrapper">
      <div class="hero-content">
        <h1 class="hero-name-line">
            SHARVITA
        </h1>
        <h1 class="hero-name-line" style="animation-delay: 0.2s;">
            PAITHANKAR
        </h1>

        <div class="hero-profile-image">
          <img src="{{ site.author.avatar }}" alt="{{ site.author.name }} Profile Picture">
        </div>
      </div>

      <p class="hero-tagline">
        AI/ML | Full-Stack Development | Cloud Engineering
      </p>

      <a href="#projects-section" class="scroll-indicator" aria-label="Scroll down to projects">
        <i class="fas fa-chevron-down fa-2x"></i>
      </a>
    </div>

    <section id="projects-section" class="projects-grid-section">
      <h2 class="projects-header">Featured Work & Projects //</h2>
      <div class="container">
        <div class="projects-grid">
          
          <div class="project-card">
            <a href="https://github.com/sharvita/financial-research-multi-agent-system" target="_blank" class="card-link">
              <div class="thumb-wrap">
                <img src="https://i.postimg.cc/9Q29rG4Y/agent-system.jpg" alt="Financial Research Agent System" class="thumb">
                <div class="thumb-overlay"></div>
              </div>
              <div class="card-body">
                <h3 class="card-title" data-text="Financial Agent System">Financial Agent System</h3>
                <p class="card-desc">Autonomous multi-agent system (LangGraph) for financial research, web scraping, and generating Pydantic-validated JSON reports.</p>
              </div>
            </a>
          </div>

          <div class="project-card">
            <a href="https://github.com/sharvita/llm-production-deploy" target="_blank" class="card-link">
              <div class="thumb-wrap">
                <img src="https://i.postimg.cc/G2F54N5T/llm-deploy.jpg" alt="Production LLM Inference Service" class="thumb">
                <div class="thumb-overlay"></div>
              </div>
              <div class="card-body">
                <h3 class="card-title" data-text="LLM Inference Service">LLM Inference Service</h3>
                <p class="card-desc">vLLM/FastAPI production service with GPU optimization, AISecOps (Toxicity Filter), Prometheus monitoring, and automated CI/CD.</p>
              </div>
            </a>
          </div>
          
          <div class="project-card">
            <a href="#" target="_blank" class="card-link">
              <div class="thumb-wrap">
                <img src="https://i.postimg.cc/y8Y95fL5/visual-grounding.jpg" alt="Visual Grounding on RefCOCOg" class="thumb">
                <div class="thumb-overlay"></div>
              </div>
              <div class="card-body">
                <h3 class="card-title" data-text="Visual Grounding Model">Visual Grounding Model</h3>
                <p class="card-desc">Computer vision model using Python, PyTorch, and Faster R-CNN to localize objects from natural language queries (65.7% accuracy).</p>
              </div>
            </a>
          </div>
          
          <div class="project-card">
            <a href="/about/#core-competencies" class="card-link">
              <div class="thumb-wrap">
                <img src="https://i.postimg.cc/Nj9vF6q9/gcp-llm-pipeline.jpg" alt="Gen AI Data Extraction Pipeline" class="thumb">
                <div class="thumb-overlay"></div>
              </div>
              <div class="card-body">
                <h3 class="card-title" data-text="Gen AI Data Pipeline">Gen AI Data Pipeline</h3>
                <p class="card-desc">Architected AI-powered data extraction on GCP leveraging LLMs (OpenAI/Claude), reducing manual data entry by 10 hours/week.</p>
              </div>
            </a>
          </div>

          <div class="project-card">
            <a href="/about/#cloud-devops" class="card-link">
              <div class="thumb-wrap">
                <img src="https://i.postimg.cc/cL1gX4k2/terraform-devops.jpg" alt="Cloud Cost Optimization" class="thumb">
                <div class="thumb-overlay"></div>
              </div>
              <div class="card-body">
                <h3 class="card-title" data-text="Cloud IaC & Optimization">Cloud IaC & Optimization</h3>
                <p class="card-desc">Provisioned infra with Terraform/Docker across AWS/Azure, optimized spending for 25% cost reduction, and maintained 99% uptime.</p>
              </div>
            </a>
          </div>

          <div class="project-card">
            <a href="/about/#full-stack-development" class="card-link">
              <div class="thumb-wrap">
                <img src="https://i.postimg.cc/ydK2Y39t/angular-react.jpg" alt="Full-Stack UI/Microservices" class="thumb">
                <div class="thumb-overlay"></div>
              </div>
              <div class="card-body">
                <h3 class="card-title" data-text="Full-Stack Trading UIs">Full-Stack Trading UIs</h3>
                <p class="card-desc">Built 15+ React/Angular UIs for trading workflows and implemented C#/.NET microservices for low-latency market data exchange.</p>
              </div>
            </a>
          </div>
          
        </div>
      </div>
    </section>

    <div style="height: 100px; text-align: center; padding-top: 50px; color: var(--muted); font-size: 14px;">
      &copy; {{ site.time | date: '%Y' }} {{ site.author.name }}. All rights reserved.
    </div>
    
</body>
</html>
