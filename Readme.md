# 🎬 StreamClipper: Fast Stream Clipping for YouTube Live

[![Status](https://img.shields.io/badge/status-active-brightgreen)]()  
[![Build](https://img.shields.io/badge/build-passing-blue)]()  
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

## ⚙️ Tech Stack

| Technology         | Badge                                                                                                                                 |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| Python             | ![Python](https://img.shields.io/badge/python-3670A0?style=flat&logo=python&logoColor=ffdd54)                                         |
| Flask              | ![Flask](https://img.shields.io/badge/flask-%23000.svg?style=flat&logo=flask&logoColor=white)                                         |
| SQLite             | ![SQLite](https://img.shields.io/badge/sqlite-07405E.svg?style=flat&logo=sqlite&logoColor=white)                                      |
| Discord Webhooks   | ![Discord](https://img.shields.io/badge/discord-webhook-blueviolet?logo=discord&logoColor=white)                                      |
| YouTube Integration| ![YouTube](https://img.shields.io/badge/youtube-%23FF0000.svg?style=flat&logo=youtube&logoColor=white)                                |

---

## ✨ What is StreamClipper?

**StreamClipper** is a lightweight, open-source alternative to [Streamsnip](https://streamsnip.com), tailored for YouTube streamers who want **automated clipping** using **Nightbot commands**. It includes **Discord integration**, ensures **full privacy**, and comes with **no usage limits**.

### ✅ Features
 
- ⏱️ Accurate clip timestamps with automatic Discord message updates  
- 🧹 Auto-deletes Discord messages when clips are removed
- 🛠️ No api key used, 100% scrape and Cookie based

---
> 💡 *Special Shoutout to [Suraj Bhari](https://surajbhari.com/), founder of [Streamsnip](https://streamsnip.com), whose work inspired this project. He provided invaluable feedback throughout the development of StreamClipper.*

---

### 🗒️ Fill this [Google Form](https://forms.gle/xtzp96MfkVup5TVq7) before adding any command so that we will integrate your clip to discord. 

---

## 🧠 Nightbot Setup Guide

### 🔹 Clipping Command - `!clip <title>`

Add the following command to Nightbot to enable clipping:

```markdown
!addcom !clip $(urlfetch https://streamclipper.onrender.com/clip/$(chatid)/$(querystring)?delay=-30)
```
---
- 🕒 You can customize the delay parameter (in seconds) by changing -30 to your desired value. If omitted, it defaults to -30.

- ✅ Make sure you have filled [Google form](https://forms.gle/xtzp96MfkVup5TVq7) mentioned above because i need those details to integrate this to your disccord.
---
### 🔹 Delete Clip Command - `!delete <clip_id`

Add this command to allow authorized users (e.g. moderators) to delete clips:

```markdown
!addcom !delete $(urlfetch https://streamclipper.onrender.com/delete/$(query)) -ul=moderator
```
---
- 🔐 The "-ul=moderator" flag restricts usage to moderators, reducing the risk of misuse.

---

## 🙋‍♂️ Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---
## 🛡️ License

📄 This project is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/).

🚫 **Commercial use is not allowed.**  
✅ You are free to share and adapt the material, as long as you:
- Give appropriate credit,
- Provide a link to the license, and
- Indicate if changes were made.

📁 See the [LICENSE](./LICENSE) file for the full legal text.

---
## 📬 Contact

Created with ❤️ by [**Ashish Jaiswal**](https://www.linkedin.com/in/ashishjaiswal2/)

- **💬 Discord: <ins>[_.iamashish__](https://discord.com/users/_.iamashish__)</ins>**
- **🐛 Issues & Feedback: <ins>[GitHub Issues](https://github.com/iamashish-1//streamclipper/issues)</ins>**



