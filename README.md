# Herb Database 🌿 | tryherbals.com

Welcome to the **Herb Database**, a free, open-source project powering [tryherbals.com](https://tryherbals.com) to share medicinal herb knowledge with the world—no logins required for privacy! Our mission is to build a comprehensive, public resource with detailed herb profiles (starting with 500, aiming for 30,000), including uses, properties, and vendor links to connect users with herbal suppliers. Hosted on GitHub and soon live on tryherbals.com, this database blends tech and nature to make herbal wisdom accessible to all.

## 📋 Project Overview

The Herb Database at [tryherbals.com](https://tryherbals.com) currently features **500 medicinal herbs** in a CSV file, with plans to expand to **30,000 herbs** across global traditions (Western, Ayurvedic, TCM, and more). Each entry includes:

- **Common Name** (e.g., Echinacea)
- **Scientific Name** (e.g., *Echinacea purpurea*)
- **Properties** (e.g., Immunostimulant, antibacterial)
- **Uses** (e.g., Treats colds, boosts immunity)
- **Precautions** (e.g., Avoid long-term use)
- **Habitat** (e.g., North America)
- **Parts Used** (e.g., Root, leaves)
- **Preparation Methods** (e.g., Tea, tincture)
- **Citations** (e.g., NCCIH, PubMed)
- **Vendor Links** (coming soon: links to trusted sellers for each herb)

Key features:
- **Free Access**: No cost to browse or use.
- **Privacy-First**: No user logins or data tracking.
- **Community-Driven**: Open to contributions from herbalists, coders, and enthusiasts.

## 📊 Current Status

- **Dataset**: `herbs_1-500.csv` contains 500 herbs (~0.5 MB).
- **Future Scale**: Targeting 30,000 herbs (~4 GB with images at 100 KB/herb).
- **Tech Stack**:
  - Data stored as CSV on GitHub.
  - Planned: SQLite/PostgreSQL database and web interface (Python/Flask or JavaScript) on tryherbals.com.
  - Hosting: GitHub Pages or VPS (e.g., DigitalOcean) via tryherbals.com.
- **Roadmap**:
  - Convert CSV to a searchable database.
  - Launch tryherbals.com with herb profiles and vendor links.
  - Enable public contributions for new herbs and updates.

## 🚀 Getting Started

### For Users
- **Explore the Data**: Download `herbs_1-500.csv` from this repository to view the current dataset.
- **Search Example**: Try Python with pandas to filter herbs:
  ```python
  import pandas as pd
  df = pd.read_csv("herbs_1-500.csv")
  print(df[df["Properties"].str.contains("anti-inflammatory", case=False, na=False)][["Common Name", "Uses"]])
