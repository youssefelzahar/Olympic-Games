# 🏅 Olympic Games — Performance Intelligence
> An end-to-end Power BI analytics dashboard covering 128 years of Olympic history (1896–2024)

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)

---

## 📊 Live Dashboard

🔗 [View on Power BI Service](https://app.powerbi.com/groups/me/reports/164f4ce0-acbf-4362-9c9c-111875006fea?ctid=ae362704-0450-46f2-ab02-2b0a1df6406d&pbi_source=linkShare)

---

## 📌 Project Overview

This Power BI report provides a comprehensive analysis of Olympic Games data — from athlete demographics and medal breakdowns to country rankings and historical trends. Built with a focus on clean data modeling, advanced DAX, and a professional corporate design.

---

## 🗂️ Report Pages

| Page | Description |
|------|-------------|
| 🏠 **Home** | Landing page with report navigation, data summary, and model overview |
| 📊 **Executive Summary** | High-level KPIs and top-line metrics across all Olympic Games |
| 🏅 **Medal Performance** | Gold, Silver & Bronze breakdown by country, sport, and year |
| 👥 **Athlete Demographics** | Age, gender, height, weight, and physical profile analysis |
| 🌍 **Country Performance** | National rankings, medal share, and geographic distribution |

---

## 📦 Dataset

| Property | Value |
|----------|-------|
| Source Table | `olympics_athletes_dataset` |
| Total Rows | 8,500 athletes |
| Columns | 30 |
| Countries | 61 |
| Sports | 33 |
| Years Covered | 1896 → 2024 (39 Olympic Games) |

### Key Columns
- `athlete_id`, `athlete_name`, `gender`, `age`, `nationality`, `country_name`
- `sport`, `event`, `games_type` (Summer / Winter), `year`, `host_city`
- `medal` (Gold / Silver / Bronze / No Medal)
- `gold_medals`, `silver_medals`, `bronze_medals`, `total_medals_won`
- `height_cm`, `weight_kg`, `is_record_holder`, `total_olympics_attended`

---

## 🛠️ Data Model

### Measures — 30 Total across 5 Display Folders

#### 👤 Athletes
| Measure | Description |
|---------|-------------|
| `Total Athletes` | Distinct count of all athletes |
| `Athletes with Medals` | Athletes who won at least one medal |
| `% Athletes with Medals` | Medal conversion rate |
| `% Female Athletes` | Share of female athletes |
| `% Male Athletes` | Share of male athletes |
| `Avg Athlete Age` | Average age across all athletes |
| `Multi-Olympic Athletes` | Athletes who competed in more than one Olympics |
| `Record Holders Count` | Athletes with Olympic or World records |
| `Youngest Medalist Age` | Youngest age among medalists |
| `Oldest Medalist Age` | Oldest age among medalists |

#### 🏅 Medals
| Measure | Description |
|---------|-------------|
| `Total Medals` | All medals won (excl. No Medal rows) |
| `Total Gold Medals` | Gold medal count |
| `Total Silver Medals` | Silver medal count |
| `Total Bronze Medals` | Bronze medal count |
| `Gold Medal Rate %` | Gold as % of total medals |
| `Gold to Silver Ratio` | Ratio of gold to silver medals |
| `Medals per Athlete` | Average medals per athlete |
| `Sport Medal Rank` | Rank of sports by total medals |
| `Top Sport by Medals` | Sport with highest medal count |

#### 🌍 Country
| Measure | Description |
|---------|-------------|
| `Total Countries` | Distinct countries in dataset |
| `Country Medal Rank` | RANKX by gold medals per country |
| `Country Gold Share %` | Country's gold as % of all gold |
| `Country Medal Share %` | Country's medals as % of all medals |

#### 📈 Trends
| Measure | Description |
|---------|-------------|
| `Medals YoY Growth %` | Medal growth vs previous Olympic cycle |
| `Cumulative Medals` | Running total of medals over time |
| `Medals This Year` | Medals in the selected year |

#### 🏃 Athlete Physical
| Measure | Description |
|---------|-------------|
| `Avg Height cm` | Average athlete height |
| `Avg Weight kg` | Average athlete weight |
| `Avg BMI` | Calculated BMI across athletes |
| `Total Sports` | Distinct sports count |

---

## 🎨 Theme & Design

- **Style:** Corporate & Professional
- **Theme File:** `Olympics_DataFlip_Style_Theme.json` (included in repo)
- **Background:** `#F5F0E8` cream/off-white
- **Accent Color:** `#F97316` orange
- **Chart Color:** `#1A1A2A` dark black bars
- **Font:** Segoe UI throughout
- **Sidebar:** Dark `#1A1A2A` with orange navigation buttons

### How to Apply Theme
1. Open `demo_file.pbix` in Power BI Desktop
2. Go to **View → Themes → Browse for themes**
3. Select `Olympics_DataFlip_Style_Theme.json`
4. Click **Apply**

---

## 🔲 Slicers

| Slicer | Field | Style |
|--------|-------|-------|
| 📅 Olympic Year | `year` | Between Slider |
| 🏟️ Games Type | `games_type` | Tile |
| 👤 Gender | `gender` | Tile |
| 🏃 Sport | `sport` | Dropdown |
| 🌍 Country | `country_name` | Dropdown |
| 🥇 Medal Type | `medal` | Tile |
| 🏆 Record Type | `is_record_holder` | Tile |

---

## 📈 Key Insights

- 🥇 **679** Gold medals awarded across all games
- 🌍 **USA** leads all-time with **2,638** total medals
- 👤 Average athlete age is **28.5 years**
- ⚖️ Average athlete BMI is **24.3**
- 🏆 **605** athletes hold Olympic or World records
- 👥 Female athletes make up **50.2%** of the dataset
- 🔄 **79.5%** of athletes have competed in more than one Olympics

---

## 🚀 How to Run Locally

1. Clone this repository
```bash
git clone https://github.com/yourusername/olympics-powerbi-dashboard.git
```

2. Open `demo_file.pbix` in **Power BI Desktop**

3. Apply the theme from `Olympics_DataFlip_Style_Theme.json`

4. Explore the 5 report pages

---

## 👤 Author

**Youssef Elzahar**
Data Analyst | Power BI Developer| Data Scientist 


---

## 📄 License

This project is for portfolio and educational purposes.