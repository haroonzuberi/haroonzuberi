![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=28&duration=3000&pause=1000&color=36BCF7&center=true&vCenter=true&width=600&lines=Full+Stack+Developer;AI+Automation+Engineer;Building+with+n8n%2C+React%2C+Python)

![Stats](https://github-readme-stats.vercel.app/api?username=YOURNAME&show_icons=true&theme=tokyonight)
![Streak](https://github-readme-streak-stats.herokuapp.com/?user=YOURNAME&theme=tokyonight)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=YOURNAME&layout=compact&theme=tokyonight)

![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB)
![Python](https://img.shields.io/badge/Python-3670A0?logo=python&logoColor=ffdd54)
![n8n](https://img.shields.io/badge/n8n-EA4B71?logo=n8n&logoColor=white)


name: Generate Snake
on:
  schedule: [{cron: "0 0 * * *"}]
  workflow_dispatch:
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk/svg-only@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: dist/github-snake-dark.svg
      - uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

![Snake](https://raw.githubusercontent.com/YOURNAME/YOURNAME/output/github-snake-dark.svg)

![Views](https://komarev.com/ghpvc/?username=YOURNAME&color=blue)
