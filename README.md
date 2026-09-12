# GP1 License (General Photography v1)

[![License: GP1](https://img.shields.io/badge/License-GP1-blue.svg)](#)

**GP1** is a friendly creator-first, human-readable copyright license designed for modern photographers and visual artists. It bridges the gap between public domain (CC0) and restrictive copyright while explicitly protecting work against modern web threats like AI dataset scraping and metadata stripping.

---

## Key Features

* **Open Non-Commercial Sharing:** Free use and adaptation with optional upfront credit (or 14-day credit upon request).
* **Fair Commercial Attribution:** Free commercial use in exchange for clear, visible credit.
* **No-AI Scraping Opt-Out:** Explicitly prohibits training generative AI / machine learning models on your work.
* **Anti-Orphan Wiping:** Mandates EXIF metadata retention to prevent platforms from stripping artist data.
* **Social-Media Native:** Tagging `@photographer_s_username` directly in posts satisfies attribution requirements.

---

## How to Apply GP1

### 1. Embedded Metadata (CLI)
Embed rights directly into your image EXIF metadata using [ExifTool](https://exiftool.org/):

```bash
# Tag a single photo
exiftool -Copyright="GP1 License (https://github.com/Hiburger/gp1-license)" -Artist="Your Name" -overwrite_original image.jpg

# Tag an entire folder
exiftool -Copyright="GP1 License (https://github.com/Hiburger/gp1-license)" -Artist="Your Name" -overwrite_original ./path/to/folder
```

---

## Frequently Asked Questions

<details>
<summary><b>For Photographers (Licensors)</b></summary>
<br>

- #### Why does GP1 ban NSFW and adult content?
The author of the GP1 License maintains a strict personal and policy stance against explicit media. GP1 was intentionally built from the ground up as a general-purpose, non-explicit framework. Applying a GP1 tag to adult or NSFW content invalidates the license entirely, leaving that content legally unlicensed under this framework.

- #### Can I revoke a GP1 license after publishing a photo?
No. Like most open-source and Creative Commons licenses, GP1 permissions are irrevocable once granted for a specific version of a file. However, if a user breaches the terms (e.g., using it commercially without attribution or training an AI model), their rights automatically terminate under Section 2.4.

- #### Does GP1 cover model releases or private property permissions?
No. GP1 only grants permissions regarding **copyright ownership** of the photograph itself. If your image features recognizable faces or private property, you are still responsible for obtaining any necessary model or location releases required by local laws.

- #### How do I prove ownership if someone strips my EXIF metadata?
Keep your unedited RAW files, original un-cropped camera exports, and git commit history. These serve as digital proof of ownership if a dispute arises.

- #### Can I dual-license my work under GP1 and another license?
Yes. As the copyright holder, you can offer your work under multiple licenses simultaneously (e.g., offering GP1 publicly while selling an exclusive, attribution-free commercial license to a client).
</details>

<details>
<summary><b>For Image Users (Licensees)</b></summary>
<br>

- #### What counts as "Commercial Use"?
Commercial use includes any application intended for commercial advantage or monetary compensation. This includes corporate websites, paid advertising, monetized YouTube videos, merchandise, printed materials for sale, or monetized blogs.

- #### Does tagging the photographer on Instagram or X satisfy attribution?
Yes. Under Section 1.3, tagging the photographer’s official social handle in the image tag, post caption, or credit line satisfies all attribution requirements for social platforms.

- #### What happens if I forget to credit a photo used non-commercially?
For non-commercial use, upfront credit is suggested but optional. However, if the photographer contacts you requesting credit, you have **14 calendar days** to add clear attribution before you are considered in breach of the license.

- #### Can I re-sell GP1 photos on stock photo sites?
No. While commercial use is allowed with attribution, re-selling standalone, un-adapted copies of GP1 photos on stock platforms or print-on-demand services without significant creative transformation misrepresents licensing terms and violates creator rights.
</details>

<details>
<summary><b>Artificial Intelligence & Metadata</b></summary>
<br>

- #### Why does GP1 prohibit AI data mining by default?
Standard legacy licenses (like Creative Commons v4.0) were written before generative AI web-scraping existed. GP1 explicitly protects creators by requiring explicit written consent before any image can be ingested into machine learning datasets.

- #### What should I do if a web platform automatically strips EXIF metadata?
If a platform strips metadata upon upload, ensure you provide visible attribution in the post text, caption, or page footer to remain compliant with Section 2.3.
</details>

<details>
<summary><b>What happens if a platform's Terms of Service conflicts with GP1?</b></summary>
<br>

#### Platform ToS vs. GP1 Scope
When you upload content to a platform, your direct user agreement with that platform governs how the platform itself operates. GP1 governs **third-party users and scrapers** who access, download, or attempt to re-use your work. While GP1 cannot override a platform ToS you directly agreed to, it prevents external companies and scrapers from taking your work off that platform for unauthorized AI training or commercial use.
</details>

<details>
<summary><b>Am I protected if I upload a GP1 photo to a site that strips EXIF data?</b></summary>
<br>

#### Native Platform Compression
Yes. Section 2.3 explicitly exempts standard automated processing by host platforms. As long as you include a caption link, profile handle (`@handle`), or GP1 notice alongside your post, third parties downloading the image remain legally bound by your GP1 attribution and AI opt-out terms.
</details>
