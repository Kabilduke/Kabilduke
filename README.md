<!---
Profile animaiton
--->

![Visitor Count](https://profile-counter.glitch.me/{Kabilduke}/count.svg)

name: Update README

on:
  push:
    branches:
      - main

jobs:
  update-readme:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout Repository
        uses: actions/checkout@v2

      - name: Update README
        run: echo $(( $(curl -s https://profile-counter.glitch.me/${{ github.repository_owner }}/count.svg | grep -oP 'title="Visitors"' | wc -l) + 1 )) > README.md


- 👋 Hi, I’m @Kabilduke
- 👀 I’m a Data Detective
- 🌱 I’m currently learning Artificial Intelligence and Data Science
- 💞️ I’m looking to collaborate on web Designing!
- 📫 How to reach me ca.kabil12@gmail.com

<!---
Kabilduke/Kabilduke is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
