<div align="center">

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 850 360" width="100%" height="100%" style="background: #090d16; border-radius: 16px; border: 1px solid #1e293b; box-shadow: 0 20px 50px rgba(0,0,0,0.6); font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'JetBrains Mono', monospace;">
  <defs>
    <!-- Gradients -->
    <linearGradient id="grad-cyan" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#00F0FF" />
      <stop offset="100%" stop-color="#7000FF" />
    </linearGradient>
    <linearGradient id="grad-text" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#38BDF8" />
      <stop offset="50%" stop-color="#818CF8" />
      <stop offset="100%" stop-color="#C084FC" />
    </linearGradient>
    <linearGradient id="badge-bg" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#1e293b" stop-opacity="0.8" />
      <stop offset="100%" stop-color="#0f172a" stop-opacity="0.9" />
    </linearGradient>
    <linearGradient id="line-glow" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#00F0FF" stop-opacity="0" />
      <stop offset="50%" stop-color="#00F0FF" stop-opacity="0.8" />
      <stop offset="100%" stop-color="#7000FF" stop-opacity="0" />
    </linearGradient>
    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="6" result="blur" />
      <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>
  </defs>

  <style>
    .terminal-header { fill: #0f172a; stroke: #1e293b; stroke-width: 1; }
    .dot-red { fill: #ef4444; }
    .dot-yellow { fill: #f59e0b; }
    .dot-green { fill: #10b981; }
    
    .title-glow {
      font-size: 38px;
      font-weight: 900;
      letter-spacing: 2px;
      fill: url(#grad-text);
      filter: drop-shadow(0 2px 12px rgba(56, 189, 248, 0.4));
    }
    
    .status-badge {
      font-size: 11px;
      font-weight: 700;
      fill: #00F0FF;
      letter-spacing: 1px;
    }
    
    .typing-text {
      font-family: 'JetBrains Mono', monospace;
      font-size: 15px;
      fill: #94A3B8;
      font-weight: 500;
    }
    
    .cursor {
      fill: #00F0FF;
      animation: blink 0.9s infinite;
    }
    @keyframes blink {
      0%, 100% { opacity: 1; }
      50% { opacity: 0; }
    }

    .pulse-circle {
      animation: pulse 2.5s infinite ease-in-out;
      transform-origin: 40px 105px;
    }
    @keyframes pulse {
      0% { r: 4px; opacity: 1; }
      50% { r: 9px; opacity: 0.3; }
      100% { r: 4px; opacity: 1; }
    }

    .metric-box {
      fill: url(#badge-bg);
      stroke: #334155;
      stroke-width: 1;
      rx: 10px;
    }
    
    .metric-val { font-size: 16px; font-weight: 800; fill: #F8FAFC; font-family: 'JetBrains Mono', monospace; }
    .metric-lbl { font-size: 11px; font-weight: 600; fill: #64748B; letter-spacing: 0.5px; }

    .glow-bar {
      animation: scan 4s infinite linear;
    }
    @keyframes scan {
      0% { transform: translateX(-100px); }
      50% { transform: translateX(700px); }
      100% { transform: translateX(-100px); }
    }
  </style>

  <!-- Window Header Bar -->
  <rect x="0" y="0" width="850" height="42" rx="16" class="terminal-header" />
  <circle cx="28" cy="21" r="5.5" class="dot-red" />
  <circle cx="46" cy="21" r="5.5" class="dot-yellow" />
  <circle cx="64" cy="21" r="5.5" class="dot-green" />
  <text x="425" y="26" text-anchor="middle" fill="#475569" font-size="12" font-weight="600" letter-spacing="1">devvx.in — bash — 850x360</text>

  <!-- Ambient background glow behind title -->
  <circle cx="425" cy="110" r="140" fill="#00F0FF" opacity="0.04" filter="url(#glow)" />
  <circle cx="425" cy="110" r="80" fill="#7000FF" opacity="0.06" filter="url(#glow)" />

  <!-- Status indicator badge -->
  <g transform="translate(330, 60)">
    <rect x="0" y="0" width="190" height="24" rx="12" fill="#0369a1" fill-opacity="0.2" stroke="#0284c7" stroke-width="0.8" />
    <circle cx="14" cy="12" r="4" fill="#00F0FF" />
    <circle cx="14" cy="12" r="4" fill="#00F0FF" class="pulse-circle" />
    <text x="26" y="16" class="status-badge">BACKEND ARCHITECT</text>
  </g>

  <!-- Hero Name Title -->
  <text x="425" y="125" text-anchor="middle" class="title-glow">SAGAR</text>

  <!-- Glowing underline divider -->
  <rect x="225" y="145" width="400" height="2" fill="url(#line-glow)" />

  <!-- Animated-style Terminal Typing Line -->
  <g transform="translate(0, 185)">
    <text x="425" y="0" text-anchor="middle" class="typing-text">
      <tspan fill="#38BDF8" font-weight="700">const</tspan> <tspan fill="#F1F5F9">stack</tspan> <tspan fill="#94A3B8">=</tspan> [<tspan fill="#A7F3D0">"Python"</tspan>, <tspan fill="#A7F3D0">"FastAPI"</tspan>, <tspan fill="#A7F3D0">"PostgreSQL"</tspan>, <tspan fill="#A7F3D0">"Docker"</tspan>, <tspan fill="#A7F3D0">"AWS"</tspan>];
    </text>
    <text x="425" y="24" text-anchor="middle" fill="#64748B" font-size="13" font-weight="500">
      Building fault-tolerant async APIs, distributed data pipelines &amp; scalable systems.
    </text>
  </g>

  <!-- 4 Capability Pillar Badges at the bottom -->
  <g transform="translate(50, 245)">
    <!-- Metric 1 -->
    <g transform="translate(0, 0)">
      <rect width="170" height="75" class="metric-box" />
      <text x="85" y="32" text-anchor="middle" class="metric-val" fill="#38BDF8">⚡ Async I/O</text>
      <text x="85" y="55" text-anchor="middle" class="metric-lbl">FASTAPI &amp; UVICORN</text>
    </g>

    <!-- Metric 2 -->
    <g transform="translate(190, 0)">
      <rect width="170" height="75" class="metric-box" />
      <text x="85" y="32" text-anchor="middle" class="metric-val" fill="#818CF8">🗄️ Relational</text>
      <text x="85" y="55" text-anchor="middle" class="metric-lbl">POSTGRES &amp; ALEMBIC</text>
    </g>

    <!-- Metric 3 -->
    <g transform="translate(380, 0)">
      <rect width="170" height="75" class="metric-box" />
      <text x="85" y="32" text-anchor="middle" class="metric-val" fill="#C084FC">🔐 Security</text>
      <text x="85" y="55" text-anchor="middle" class="metric-lbl">JWT &amp; RBAC CONTROL</text>
    </g>

    <!-- Metric 4 -->
    <g transform="translate(570, 0)">
      <rect width="170" height="75" class="metric-box" />
      <text x="85" y="32" text-anchor="middle" class="metric-val" fill="#00F0FF">☁️ DevOps</text>
      <text x="85" y="55" text-anchor="middle" class="metric-lbl">DOCKER &amp; AWS CLOUD</text>
    </g>
  </g>
</svg>

<br/>

<!-- Modern Pill Buttons (Centered, No ugly blue links) -->
<p align="center">
  <a href="https://devvx.in" target="_blank">
    <img src="https://img.shields.io/badge/🌐_WEBSITE-devvx.in-090D16?style=for-the-badge&logoColor=00F0FF" alt="Website" />
  </a>
  &nbsp;&nbsp;
  <a href="https://linkedin.com" target="_blank">
    <img src="https://img.shields.io/badge/💼_LINKEDIN-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  &nbsp;&nbsp;
  <a href="mailto:contact@devvx.in">
    <img src="https://img.shields.io/badge/📫_EMAIL-Contact_Me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
</p>

</div>

---

### ⚡ System Profile & Architecture

```python
from dataclasses import dataclass
from typing import List

@dataclass(frozen=True)
class Engineer:
    identity: str = "Sagar"
    role: str = "Backend Software Engineer"
    specialization: str = "Async RESTful Systems & High-Throughput Microservices"
    
    # Core Stack
    languages: List[str] = ("Python (Asyncio)", "SQL (PostgreSQL)", "JavaScript")
    frameworks: List[str] = ("FastAPI", "Pydantic v2", "SQLAlchemy 2.0", "Alembic")
    infrastructure: List[str] = ("Docker Containers", "AWS Cloud", "Redis Caching")
    
    def value_proposition(self) -> str:
        return "I build clean, typed, high-performance backends that don't break at 3 AM."
```

---

### 🛠️ Production Tech Stack

<div align="center">

| Domain | Production Tools & Technologies |
| :--- | :--- |
| **⚡ Backend & APIs** | `Python 3.12` • `FastAPI` • `Pydantic` • `Uvicorn ASGI` • `AsyncIO` • `Jinja2` |
| **🗄️ Databases & Storage** | `PostgreSQL` • `SQLAlchemy ORM` • `Alembic Migrations` • `MongoDB` • `Redis` |
| **🔐 Auth & Security** | `JWT Bearer Tokens` • `Bcrypt Hashing` • `Role-Based Access Control (RBAC)` |
| **☁️ Cloud & DevOps** | `Docker Multi-Stage` • `AWS (EC2/S3)` • `Render` • `Vercel` • `Git CI/CD` |
| **🧠 Engineering Core** | `Data Structures & Algorithms` • `System Design Patterns` • `RESTful Standards` |

</div>

---

### 🚀 What I Bring to Your Team

```
┌── 🎯 01. PRODUCTION-READY ASYNC APIS
│   Write clean FastAPI services with strict Pydantic schemas, dependency injection, and autogenerated OpenAPI specs.
│
├── 🗄️ 02. SCALABLE DATABASE DESIGN
│   Expert in PostgreSQL normalization, connection pooling, optimized indexing, and zero-downtime Alembic migrations.
│
├── 🔐 03. ZERO-TRUST SECURITY ARCHITECTURE
│   Bulletproof auth flows using JWT tokens, salted Bcrypt password hashing, and granular multi-role RBAC authorization.
│
└── ☁️ 04. CLOUD & CONTAINERIZED INFRASTRUCTURE
    Package lightweight multi-stage Docker containers ready for AWS or modern cloud deploy with continuous reliability.
```

---

<div align="center">
  <sub><code>Designed with 100% self-contained SVG &amp; Dark Glassmorphism aesthetic. No broken external CDNs.</code></sub>
</div>
