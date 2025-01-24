## Hi there 👋
- :santa: Hi, I’m @HaonanGe
- :blush: I’m interested in Machine Learning, Computer Vision.  And I decided to learn coding from 2025.01.19.
- 🌱 I’m currently a third year BS ECE student @SEU, 26Fall USA.
![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=Johnny040216)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Johnny040216)
# Visit https://github.com/lowlighter/metrics#-documentation for full reference
name: Metrics
on:
  # Schedule updates (each hour)
  schedule: [{cron: "0 * * * *"}]
  # Lines below let you run workflow manually and on each commit
  workflow_dispatch:
  push: {branches: ["master", "main"]}
jobs:
  github-metrics:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - uses: lowlighter/metrics@latest
        with:
          # Your GitHub token
          # The following scopes are required:
          #  - public_access (default scope)
          # The following additional scopes may be required:
          #  - read:org      (for organization related metrics)
          #  - read:user     (for user related data)
          #  - read:packages (for some packages related data)
          #  - repo          (optional, if you want to include private repositories)
          token: ${{ secrets.METRICS_TOKEN }}

          # Options
          user: Johnny040216
          template: classic
          base: header, activity, community, repositories, metadata
          config_timezone: Asia/Shanghai
<!--
**Johnny040216/Johnny040216** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
