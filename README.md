<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&height=100&section=header&text=Greetings,%20Code%20Architect%20%26%20Digital%20Explorer!%20%F0%9F%9A%80&fontSize=30" alt="header"/>
</p>

## 💻 About Me

```yaml
- Role: Full Stack Developer & Ethical Hacker
- Specialty: Building secure, scalable applications and blockchain solutions (Move).
- Learning: Advanced network penetration testing techniques.
- Collaborate: Open to collaboration on full-stack projects or security research.
- Ask me: Anything about JavaScript, Node.js, security, or API design.
- Contact: [x.com/_buzzdotsui](https://x.com/_buzzdotsui)
🛠️ Tools & Tech Stack
<p align="left">

Frontend & General Web
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="HTML5" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="CSS3" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="JavaScript" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" alt="TypeScript" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" alt="React" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/redux/redux-original.svg" alt="Redux" width="45" height="45"/>

Backend & Core Infrastructure
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original.svg" alt="Node.js" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" alt="Docker" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jest/jest-plain.svg" alt="Jest" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" alt="SQL/PostgreSQL" width="45" height="45"/>
<img src="https://img.shields.io/badge/Prisma-3982AE?style=for-the-badge&logo=prisma&logoColor=white" alt="Prisma" height="45" width="auto"/>
<img src="https://img.shields.io/badge/Move-1e7d9b?style=for-the-badge&logo=apts&logoColor=white" alt="Move" height="45" width="auto"/>
<img src="https://www.google.com/search?q=https://img.shields.io/badge/REST-0059C8%3Fstyle%3Dfor-the-badge%26logo%3Djsonplaceholder%26logoColor%3Dwhite" alt="REST" height="45" width="auto"/>
<img src="https://www.google.com/search?q=https://img.shields.io/badge/JWT-black%3Fstyle%3Dfor-the-badge%26logo%3DJSON%2520web%2520tokens" alt="JWT" height="45" width="auto"/>

Tools & Deployment
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" alt="Git" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" alt="GitHub" width="45" height="45"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/githubactions/githubactions-original.svg" alt="GitHub Actions" width="45" height="45"/>
<img src="https://img.shields.io/badge/Render-%46E3B7.svg?style=for-the-badge&logo=render&logoColor=white" alt="Render" height="45" width="auto"/>

🔒 Security & Networking Focus
<img src="https://www.google.com/search?q=https://img.shields.io/badge/Ethical%2520Hacker-00FF85%3Fstyle%3Dfor-the-badge%26logo%3Dkalilinux%26logoColor%3Dblack" alt="Ethical Hacking" height="45" width="auto"/>
<img src="https://www.google.com/search?q=https://img.shields.io/badge/Networking-DD0031%3Fstyle%3Dfor-the-badge%26logo%3Dwireshark%26logoColor%3Dwhite" alt="HTTP/DNS/Ports" height="45" width="auto"/>

</p>

📈 My GitHub Activity
<p align="center">
<img src="https://www.google.com/search?q=https://github-readme-stats.vercel.app/api%3Fusername%3Dbuzzdotsui%26show_icons%3Dtrue%26theme%3Dvue%26hide_border%3Dtrue%26count_private%3Dtrue" alt="buzzdotsui's GitHub Stats" />

<img src="https://www.google.com/search?q=https://github-readme-stats.vercel.app/api/top-langs/%3Fusername%3Dbuzzdotsui%26layout%3Dcompact%26theme%3Dvue%26hide_border%3Dtrue" alt="buzzdotsui's Top Languages" />
</p>

🏆 My GitHub Contribution Snake

***

## 2. `.github/workflows/main.yml` (The Automation File)

This file should be saved in your repository under the path: **`.github/workflows/main.yml`**.

```yaml
name: Generate Datas
on:
  schedule: # execute every 12 hours
    - cron: "0 0,12 * * *" # Runs at 00:00 UTC and 12:00 UTC
  workflow_dispatch: # Allows manual run from the Actions tab

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@v3
        id: snake-gif
        with:
          github_user_name: buzzdotsui # Your username is here!
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output # This is the branch where the SVG is saved
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }} # This token is provided automatically