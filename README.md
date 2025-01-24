## Hi there 👋
- :santa: Hi, I’m @HaonanGe
- :blush: I’m interested in Machine Learning, Computer Vision.  And I decided to learn coding from 2025.01.19.
- 🌱 I’m currently a third year BS ECE student @SEU, 26Fall USA.
name: Metrics
on:
  # Schedule daily updates
  schedule: [{ cron: "0 0 * * *" }]
  # (optional) Run workflow manually
  workflow_dispatch:
  # (optional) Run workflow when pushing on master/main
  push: { branches: ["master", "main"] }
jobs:
  github-metrics:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - uses: lowlighter/metrics@latest
        with:
          token: ${{ secrets.METRICS_TOKEN }}
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
