<div align="center">

# Hi, I'm Aniket 👋

**Building Myself | CSE (AI/ML) '29 | Filmmaker and Developer**
</div>
name: 3D Profile Contribution Graph

on:
  schedule:
    - cron: "0 0 * * *"  # runs once a day
  workflow_dispatch:      # lets you trigger it manually too

jobs:
  build:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - uses: actions/checkout@v4
      - uses: yoshi389111/github-profile-3d-contrib@0.7.1
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
        with:
          username: aniketm112
      - name: Commit and push
        run: |
          git config user.name github-actions
          git config user.email github-actions@github.com
          git add -f ./profile-3d-contrib/*.svg
          git commit -m "Update 3D contribution graph" || echo "No changes"
          git push

<table>
<tr>
<td valign="top" width="50%">

```yaml
aniket@github
─────────────────────────────────────
OS: ..................... Mumbai, India
Role: .................... Co-Founder @ Adtekro
Field: ................... B.Tech CSE (AI/ML), 2nd Year
Base: ..................... Mumbai, India

Focus.Primary: ........... DSA (C++) | Coding
Focus.Secondary: ......... ML Projects | Open Source
Goal: ..................... Microsoft / Google Internship

Background: .............. Filmmaking, Video Editing,
                            Content Creation

Languages.Programming: ... C++, Java, Python
Languages.Web: ........... HTML, CSS, JavaScript

Tools: .................... VS Code, MSYS2/GCC, Git

─────────────────────────────────────
Contact
Instagram: ............... @whyanikett
Company: .................. Adtekro
─────────────────────────────────────
```

</td>
<td valign="top" width="50%">

### 🚀 What I'm Doing

- 🎯 Grinding **DSA** with the LeetCode
- 🏗️ Co-building **Adtekro** — a digital agency for marketing + web/app dev
- 🎥 Creating cinematic, story-driven content on Instagram and Youtube

### 🛠️ Tech Stack

![C++](https://img.shields.io/badge/-C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/-Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![HTML5](https://img.shields.io/badge/-HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/-CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![Git](https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white)

</td>
</tr>
</table>

<div align="center">

### 🌐 Connect With Me

[![Instagram](https://img.shields.io/badge/-Instagram-E4405F?style=flat-square&logo=instagram&logoColor=white)](https://instagram.com/whyanikett)

</div>
