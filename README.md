## Hi there 👋

<!--
**HelderHub/HelderHub** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

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

<!-- Visitor count -->
<div align="center"> 
  <p>Visitor count</p>
  <img src="https://profile-counter.glitch.me/{HelderHub}/count.svg" alt="Visitor's Count" />
</div>

<!-- Visitor count -->


<!-- Banner -->

<img src="https://github.com/{HelderHub}/{HelderHub}/blob/main/software-developer.png" alt="Banner of a developer sitting in front of a desk">

<!-- Banner -->

<!-- Hi There animation -->

<h1 align="center">
    <img src="https://readme-typing-svg.herokuapp.com/?font=Inter&size=48&center=true&vCenter=true&width=500&height=70&color=4493F8&duration=4000&lines=Hi+There!+👋;+I'm+Hélder+Fernandes!;" />
</h1>

<!-- Hi There animation -->


<!-- Badges -->

- 🌱 I’m currently learning **[System Design](https://blog.bytebytego.com/p/free-system-design-pdf-158-pages)**
- 💬 Ask me about **Java, Node.js, React...or anything [here](https://github.com/{USERNAME}/{USERNAME}/issues)**

<br>
<div align="center">
  <a href="helderfernandeswork@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-333333?style=for-the-badge&logo=gmail&logoColor=red" />
  </a>
  <a href="https://linkedin.com/in/helderfernandes101" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank" />
  </a>
  <a href="https://medium.com/@helderfernandes" target="_blank">
    <img src="https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white" target="_blank" />
  </a>
  <a href="https://codepen.io/helderfernandes" target="_blank">
    <img src="https://img.shields.io/badge/CodePen-1e1f26?style=for-the-badge&logo=codepen&logoColor=white" target="_blank" />
  </a>
</div>
<hr>

<!-- Badges -->

<!-- Skillicons -->

## 🛠️ Languages and Tools

<br>

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,ts,nodejs,react,nextjs,mongodb,postgres,prisma" />
  <img src="https://skillicons.dev/icons?i=html,css,sass,tailwind,js,vue,redux,d3,git,postman,figma" />
</p>

<hr>

<!-- Skillicons -->

<!-- User stats -->

## ⚡️ Stats

<br>

<div align=center>
  <img width=390 src="https://github-readme-stats.vercel.app/api?username=HelderHub&theme=transparent&count_private=true&show_icons=true&rank_icon=github&locale=en" alt="Hélder's GitHub Stats" />
  <img width=390 src="https://github-readme-streak-stats.herokuapp.com/?user=HelderHub&theme=transparent&count_private=true&border_radius=10&locale=en" alt="Hélder's" />
  <img width=325 src="https://github-readme-stats.vercel.app/api/top-langs?username=HelderHub&theme=transparent&layout=donut&hide=css&langs_count=8&border_radius=10&show_icons=true&locale=en" alt="Hélder's Most Used Languages" />
</div>

<hr>

<!-- User stats -->

<!-- Snake -->

<!-- tutorial

create a generate-snake.yml file in the .github/workflows/ directory.
paste below ----------------------------------------------------------------------------------------------------------------------------------
# GitHub Action for generating a contribution graph with a snake eating your contributions.
name: Generate Snake

# Controls when the action will run.
on:
  schedule:
      # every 12 hours
    - cron: "0 */12 * * *"

  # This command allows us to run the Action automatically from the Actions tab.
  workflow_dispatch:
  
  # Also run on every push on the main branch
  push:
    branches:
    - main

# The sequence of runs in this workflow:
jobs:
  # This workflow contains a single job called "build"
  build:
    # The type of runner that the job will run on
    runs-on: ubuntu-latest

    # Steps represent a sequence of tasks that will be executed as part of the job
    steps:
      - name: Clone repo
        uses: actions/checkout@v3
    
      - name: Generate the snake files in './dist/'
        uses: Platane/snk@v3
        id: snake-gif
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark
            dist/github-contribution-grid-snake.gif?color_snake=orange&color_dots=#bfd6f6,#8dbdff,#64a1f4,#4b91f1,#3c7dd9
        env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

      - name: Show build status
        run: git status

      - name: Push new files to the output branch
        uses: crazy-max/ghaction-github-pages@v3.1.0
        with:
          target_branch: output
          build_dir: dist
          commit_message: Update snake animations
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
paste above ----------------------------------------------------------------------------------------------------------------------------------
end tutorial -->


## 🐍 My Contributions

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/{HelderHub}/{HelderHub}/output/github-contribution-grid-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/{HelderHub}/{HelderHub}/output/github-contribution-grid-snake.svg" />
    <img alt="github-snake" src="https://raw.githubusercontent.com/{HelderHub}/{HelderHub}/output/github-contribution-grid-snake.svg" />
  </picture>
</div>

<hr>

<!-- Snake -->

<!-- Links -->

<!-- tutorial
create a new blog-post.yml file in the .github/workflows/ directory.

paste below ----------------------------------------------------------------------------------------------------------------------------------
name: Latest blog post workflow
on:
  schedule: # Run workflow automatically
    - cron: '0 * * * *' # Runs every hour, on the hour
  workflow_dispatch: # Run workflow manually (without waiting for the cron to be called), through the GitHub Actions Workflow page directly
permissions:
  contents: write # To write the generated contents to the readme

jobs:
  update-readme-with-blog:
    name: Update this repo's README with latest blog posts
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v4
      - name: Pull in dev.to posts
        uses: gautamkrishnar/blog-post-workflow@v1
        with:
          feed_list: "https://medium.com/feed/@chijiokeokorji"
paste above ----------------------------------------------------------------------------------------------------------------------------------
 end tutorial -->
## 📕 Latest Blog Posts
<!-- BLOG-POST-LIST:START -->
<!-- BLOG-POST-LIST:END -->

<!-- Links -->



