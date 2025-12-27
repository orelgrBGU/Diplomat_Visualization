
#  Data Visualization Project 
## Authors

**Shachar Ophir  206442121**

**Orel Grinberg   208891994**

**Ram Hirsch        207806795**  



![Logo](https://github.com/orelgrBGU/Diplomat_Visualization/blob/main/%D7%9C%D7%95%D7%92%D7%95.jpg?raw=true)



![App Screenshot](https://github.com/orelgrBGU/Diplomat_Visualization/blob/main/%D7%AA%D7%9E%D7%95%D7%A0%D7%94%20%D7%A9%D7%A2%D7%A8.png?raw=true)

## תקציר על חברת דיפלומט

חברת דיפלומט היא מהחברות המובילות בישראל ביבוא והפצת מוצרי צריכה. החברה משווקת מותגים בינלאומיים מרכזיים בתחומי הטואלטיקה, ההיגיינה והמזון, בהם **Pampers, Gillette, Oral-B, Head & Shoulders, Always, Fairy, Pringles, Heinz, Kellogg’s** ועוד.

דיפלומט מפעילה מערך סוכנים רחב המבקר מדי יום ברשתות שיווק, סופרמרקטים ומכולות ברחבי הארץ. הנתונים בפרויקט משקפים את פעילות השטח הזו: **ביקורים בפועל, זמני ביקור, הזמנות ומכירות לפי עיר**.

ניתוח הנתונים מאפשר לזהות דפוסים, מגמות ויחסי גומלין בין מאמץ בשטח לבין תוצאות מכירה. מטרת הוויזואליזציות היא להציג את התובנות בצורה אינטואיטיבית וברורה, ולחשוף פערים שלא ניתן לראות מתוך הטבלאות בלבד.

## תיאור הנתונים והטיפול בהם
מאגר הנתונים ששימש בפרויקט התקבל מחברת דיפלומט ומתאר את פעילות הסוכנים מול נקודות המכירה ברחבי הארץ במהלך החודשים ינואר–יולי 2025. הנתונים כוללים פרטים על ביקורים מתוכננים וביקורים שבוצעו בפועל, זמני התחלה וסיום, סוגי חנויות, מספר ההזמנות שבוצעו, סכומי מכירה נטו, כמות הקרטונים והיחידות שסופקו ועוד. לפני ביצוע הוויזואליזציות עברו הנתונים תהליך עיבוד שכלל ניקוי חוסרים, אחידות של תאריכים ושעות, סינון ביקורים שלא התקיימו, טיפול בערכים חריגים והתאמת הנתונים לצורכי הניתוח. שלב זה איפשר להפיק תמונה מהימנה ומדויקת יותר של פעילות הסוכנים ודפוסי המכירה שעליה מתבססים הגרפים.

## הנתונים 
### דוגמית מתוך הDataSet

<div style="max-height: 300px; overflow-y: auto; border: 1px solid #ccc; padding: 10px;">

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th>Date</th>
      <th>Year</th>
      <th>Month</th>
      <th>מספר סוכן</th>
      <th>מנהל סוכן</th>
      <th>ערוץ</th>
      <th>מס לקוח</th>
      <th>מס משלם</th>
      <th>עיר</th>
      <th>מס הזמנה</th>
      <th>סוג ביקור</th>
      <th>זמן התחלה</th>
      <th>זמן סיום</th>
      <th>האם תוכנן</th>
      <th>האם תוכנן ובוצע</th>
      <th>האם ביקר בפועל</th>
      <th>זמן ביקור</th>
      <th>First City</th>
      <th>Last City</th>
      <th># Total Orders</th>
      <th>סכום נטו הזמנה</th>
      <th>סהכ יחידות בהזמנה</th>
      <th>סהכ קרטונים בהזמנה</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>2025-04-27</td>
      <td>2025</td>
      <td>APR</td>
      <td>1</td>
      <td>manager1</td>
      <td>channel1</td>
      <td>117231010</td>
      <td>000643010</td>
      <td>פתח תקווה</td>
      <td>-</td>
      <td>Fisical</td>
      <td>06:29:46</td>
      <td>08:43:19</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>06:29-08:43</td>
      <td>פתח תקווה</td>
      <td>פתח תקווה</td>
      <td>0</td>
      <td>0.000000</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <td>2025-03-19</td>
      <td>2025</td>
      <td>MAR</td>
      <td>1</td>
      <td>manager1</td>
      <td>channel1</td>
      <td>164521010</td>
      <td>020983010</td>
      <td>חולון</td>
      <td>6065431693</td>
      <td>Phone</td>
      <td>08:00:05</td>
      <td>08:02:13</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>08:00-08:02</td>
      <td>חולון</td>
      <td>-</td>
      <td>1</td>
      <td>2508.516741</td>
      <td>87</td>
      <td>16</td>
    </tr>
    <tr>
      <td>2025-03-19</td>
      <td>2025</td>
      <td>MAR</td>
      <td>1</td>
      <td>manager1</td>
      <td>channel1</td>
      <td>164521010</td>
      <td>020983010</td>
      <td>חולון</td>
      <td>-</td>
      <td>Phone</td>
      <td>08:00:05</td>
      <td>08:02:13</td>
      <td>0</td>
      <td>0</td>
      <td>1</td>
      <td>08:00-08:02</td>
      <td>חולון</td>
      <td>-</td>
      <td>0</td>
      <td>0.000000</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <td>2025-02-16</td>
      <td>2025</td>
      <td>FEB</td>
      <td>1</td>
      <td>manager1</td>
      <td>channel1</td>
      <td>140311010</td>
      <td>000643010</td>
      <td>ראשון לציון</td>
      <td>-</td>
      <td>Fisical</td>
      <td>08:03:40</td>
      <td>11:25:25</td>
      <td>1</td>
      <td>1</td>
      <td>1</td>
      <td>08:03-11:25</td>
      <td>ראשון לציון</td>
      <td>-</td>
      <td>0</td>
      <td>0.000000</td>
      <td>0</td>
      <td>0</td>
    </tr>


  </tbody>
</table>

</div>

-
## ויזואליזציה 1 
## מודל WWH – הסבר על הוויזואליזציה

<table dir="rtl">
  <thead>
    <tr>
      <th>רכיב</th>
      <th>תוכן</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>What – מה מוצג?</strong></td>
      <td>
 הגרף מציג את התפלגות הביקורים שבוצעו בפועל אצל לקוחות במהלך היום, בין השעות 07:00 ל־19:00. לכל ביקור חישבנו את משך הזמן בדקות,סיווגנו כל ביקור לשלוש קטגוריות זמן: ביקור קצר מאוד (“Touch & Go” – עד 10 דקות), ביקור סטנדרטי יעיל (10–45 דקות) וביקור ארוך או תקוע (מעל 45 דקות). בגרף רואים עבור כל שעה כמה ביקורים התרחשו, וכמה מהם שייכים לכל אחת משלוש הקטגוריות הללו.
      </td>
    </tr>
    <tr>
      <td><strong>Why – למה בחרנו בגרף הזה?</strong></td>
      <td>
הגרף מאפשר לזהות באילו שעות היום יש נפח ביקורים גבוה במיוחד, האם בשעות השיא יש בעיקר ביקורים קצרים ויעילים או דווקא הרבה ביקורים ארוכים, והאם יש חלונות זמן שבהם הסוכנים “נתקעים” אצל לקוחות על חשבון לקוחות אחרים ויכול לאפשר כמשוב לניהול זמן נכון יותר.
      </td>
    </tr>
    <tr>
      <td><strong>How – איך הגרף מציג את הנתונים?</strong></td>
      <td>
   הגרף הוא Stacked Bar Chart: בציר האופקי מופיע נתון אורדינלי על שעות היום (07:00–19:00), בציר האנכי מוצג מספר הביקורים בפועל. כל עמודה מייצגת את כלל הביקורים שנעשו באותה שעה, והעמודה מחולקת לפי צבעים  מוערמים בהתאם לקטגוריית משך הביקור שניתן לראות בו־זמנית גם את סך כל הביקורים בכל שעה וגם את ההרכב הפנימי שלהם.

   
  
  </tbody>
</table>

<details>
<summary><strong>לחץ להצגת הקוד המלא (Python)</strong></summary>

<br>

```python
import pandas as pd
import matplotlib.pyplot as plt
import io

# ==========================================
# STEP 2: Data Preprocessing
# ==========================================

# Filter: Keep only rows where an actual visit took place
df_visits = df[df['האם ביקר בפועל'] == 1].copy()

# Time Conversion: Convert string time columns to datetime objects
df_visits['start_dt'] = pd.to_datetime(df_visits['זמן התחלה'], format='%H:%M:%S', errors='coerce')
df_visits['end_dt'] = pd.to_datetime(df_visits['זמן סיום'], format='%H:%M:%S', errors='coerce')

# Calculate Duration: Compute visit length in minutes
df_visits['duration_mins'] = (df_visits['end_dt'] - df_visits['start_dt']).dt.total_seconds() / 60

# Data Cleaning:
# Remove errors (<=0) and outliers (>300 mins)
df_visits = df_visits[(df_visits['duration_mins'] > 0) & (df_visits['duration_mins'] < 300)]

# Extract Hour
df_visits['Hour'] = df_visits['start_dt'].dt.hour

# Filter Hours: Focus ONLY on 07:00 to 19:00
df_visits = df_visits[(df_visits['Hour'] >= 7) & (df_visits['Hour'] <= 19)]

# ==========================================
# STEP 3: Categorization Logic (The Story)
# ==========================================
def classify_duration(mins):
    if mins <= 10:
        return '1. Touch & Go (<10m)'      # Short visits
    elif mins <= 45:
        return '2. Standard Work (10-45m)' # Effective time
    else:
        return '3. Deep/Stuck (>45m)'      # Long visits

df_visits['Duration_Category'] = df_visits['duration_mins'].apply(classify_duration)

# ==========================================
# STEP 4: Visualization
# ==========================================

# Prepare Data: Group by Hour and Category
pivot_duration = df_visits.groupby(['Hour', 'Duration_Category']).size().unstack(fill_value=0)

# Define Pastel Colors
pastel_colors = ['#aec7e8', '#98df8a', '#ff9896']

# Create Plot
plt.figure(figsize=(14, 7))
pivot_duration.plot(kind='bar', stacked=True, ax=plt.gca(), color=pastel_colors, width=0.85)
hours = pivot_duration.index  # שעות 7–19

plt.xticks(
    ticks=range(len(hours)),
    labels=[f"{h}:00" for h in hours],
    rotation=0
)

# Styling
plt.title('Visit Duration Analysis: 07:00 - 19:00', fontsize=16, fontweight='bold', color='#333333')
plt.xlabel('Hour of Day', fontsize=20)
plt.ylabel('Number of Visits', fontsize=20)

leg = plt.legend(title="Visit Duration Type")
for text in leg.get_texts():
    text.set_fontsize(16)
leg.get_title().set_fontsize(16)

for patch in leg.get_patches():
    patch.set_width(20)
    patch.set_height(12)

plt.grid(axis='y', alpha=0.3, linestyle='--', color='gray')
plt.xticks(rotation=0)
plt.xticks(fontsize=16)
plt.yticks(fontsize=16)
plt.tight_layout()

print("Generating chart...")
plt.show()
```
</details>

<br>

### 📊 Visualization Output (Screenshot)

<div align="center">
  <img src="https://github.com/orelgrBGU/Diplomat_Visualization/blob/main/duration_plot1.png?raw=true"
       alt="Visit Duration Visualization"
       width="80%"
       style="border: 1px solid #ccc; border-radius: 8px;">
</div>

<br>

## הסבר על הגרף 

  הויזואליזציה  היא מאפשרת לנו לראות ששעות השיא (10:00-13:00) אינן מתאפיינות רק בכמות ביקורים גבוהה אלא גם על מעידים על פגישות ארוכות מדיי של סוכנים בסניפים. לעומת זאת, ככל שמתקרבים לסוף היום (החל מ-16:00), הגרף ממחיש דעיכה העמודות לא רק מתנמכות, אלא משנות את צבען לכחול דומיננטי  מה שמעיד על לחץ אולי לסיים את העבודה מהר ולהגיע הביתה או שאולי אנשי הממשק הנדרשים נמצאים יותר בשעות הצהריים ושם יש ריכוז מאמץ על ההזמנות אולי שווה לשקול שסוכנים יפוזורו יותר בשעות הצהריים מאשר בשעות הערב.


# ויזואליזציה 2
## מודל WWH – הסבר על הוויזואליזציה

<table dir="rtl">
  <thead>
    <tr>
      <th>רכיב</th>
      <th>תוכן</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>What – מה מוצג?</strong></td>
      <td>
הגרף מציג את התפלגות גובה העסקאות (Deal Size Distribution) בקרב עשרת הסוכנים המובילים בחברה. לכל סוכן מוצגת עקומת צפיפות (Density Plot) הממחישה את השכיחות של סכומי העסקה השונים, לצד נתונים מסכמים קריטיים: החציון האישי של הסוכן (קו לבן מרוסק), החציון הגלובלי של כלל החברה (קו אפור אנכי) ומספר העסקאות הכולל (N). הסוכנים מסודרים בציר האנכי לפי גובה החציון שלהם, בסדר יורד מהגבוה לנמוך.
      </td>
    </tr>
    <tr>
      <td><strong>Why – למה בחרנו בגרף הזה?</strong></td>
      <td>
המטרת הגרף היא לחשוף את "אישיות המכירה" של הסוכנים ולא להסתפק רק בשורת ההכנסה הסופית. הגרף מאפשר להבחין בצורה אינטואיטיבית בין סוכנים "ציידים" (המבצעים מעט עסקאות בשווי גבוה) לבין סוכנים "חקלאים" (המבססים את המחזור על נפח עצום של עסקאות קטנות). תצוגה זו נבחרה כי היא מונעת את העומס הוויזואלי שהיה נוצר בהצגת עשר היסטוגרמות נפרדות, ומאפשרת השוואה אנכית מיידית של יעילות המכירה מול הממוצע הארגוני.
      </td>
    </tr>
    <tr>
      <td><strong>How – איך הגרף מציג את הנתונים?</strong></td>
      <td>
  הוויזואליזציה בנויה כתרשים Ridge Plot (או Joyplot). ציר ה-X הוא ציר כמותי רציף המציג את סכום העסקה בשקלים, לאחר שעבר סינון של עסקאות זניחות (מתחת ל-50 ₪) וחיתוך (Zoom) באחוזון ה-96 כדי למנוע עיוות על ידי ערכי קיצון. הציר האנכי מפוצל לשורות נפרדות לכל סוכן (Faceting), כאשר עקומות הצפיפות חופפות מעט כדי לחסוך מקום ולייצר רצף ויזואלי. קו הייחוס הגלובלי ("Global Med") עובר לרוחב כל הגרפים ומספק בסיס קבוע להשוואת ביצועים.

   
  
  </tbody>
</table>

<details>
<summary><strong>לחץ להצגת הקוד המלא (Python)</strong></summary>

<br>

```python
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd
import numpy as np
from matplotlib.ticker import FuncFormatter
from scipy.stats import gaussian_kde

df.rename(columns={'סכום נטו הזמנה ': 'NetAmount', 'ערוץ ': 'Channel', 'מספר סוכן ': 'AgentID'}, inplace=True)

# Filter out noise (>50), keeping top outliers for accurate stats calculation
orders = df[df['NetAmount'] > 50].copy()
orders['AgentID_Str'] = "Agent " + orders['AgentID'].astype(str)

# Agent Selection & Sorting
# Select Top 10 agents by Total Revenue
top_agents_list = orders.groupby('AgentID_Str')['NetAmount'].sum().sort_values(ascending=False).head(10).index
data_agent = orders[orders['AgentID_Str'].isin(top_agents_list)].copy()

# Sort agents by Median deal size (Descending)
median_order = data_agent.groupby('AgentID_Str')['NetAmount'].median().sort_values(ascending=False).index

#  Global Benchmarks
global_median = data_agent['NetAmount'].median()

# Set visual limit for X-axis (Zoom to 96% to hide extreme outliers in the plot)
viz_xlim = data_agent['NetAmount'].quantile(0.96)

#  Styling & Plotting
sns.set_theme(style="white", rc={"axes.facecolor": (0, 0, 0, 0)})
joy_color = "#2c7fb8"

# Main plotting function for Density Estimation
def draw_comprehensive_density(x, label=None, color=None):
    ax = plt.gca()
    data = x.values
    if len(data) < 2: return

    # Calculate statistics based on FULL data
    N = len(data)
    med = np.median(data)

    # Calculate KDE (Kernel Density Estimation)
    density = gaussian_kde(data)
    xs = np.linspace(0, viz_xlim, 300) # Plot only within visual limits
    ys = density(xs)

    # Draw density area and white outline
    ax.fill_between(xs, ys, color=color, alpha=1.0, zorder=2)
    ax.plot(xs, ys, color='white', lw=2, zorder=3)

    # Draw specific agent's median line (inside the plot)
    med_height = density(med)[0]
    if med < viz_xlim:
        ax.plot([med, med], [0, med_height], color='white', linestyle='--', lw=1.5, zorder=4)

    # Draw Global Median line (Benchmark)
    ax.axvline(global_median, color='#6c757d', linestyle='--', lw=1.5, alpha=0.8, zorder=5)

    # Base line
    ax.axhline(0, color="#333333", lw=1, zorder=5)

    # Add Text Labels
    # Left side: Agent Name + Count (N)
    label_text = f"{label}\n(N={N})"
    ax.text(-0.01, 0.25, label_text, fontweight="bold", color="#333333", fontsize=10,
            ha="right", va="center", transform=ax.transAxes, zorder=10)

    # Right side: Stats Table (Median Only)
    stats_text = f" ₪{med:,.0f}"
    ax.text(1.02, 0.25, stats_text, fontweight="bold", color="#2c7fb8", fontsize=10,
            ha="left", va="center", transform=ax.transAxes, zorder=10)

#  Initialize Grid
g = sns.FacetGrid(data_agent, row='AgentID_Str', hue='AgentID_Str',
                  aspect=10, height=1.3, row_order=median_order)

g.map(draw_comprehensive_density, 'NetAmount', color=joy_color)

#  Final Layout & Annotations

# Add headers for the Stats column (on the first plot)
top_ax = g.axes.flat[0]
top_ax.text(1.02, 0.7, "MEDIAN", fontweight="bold", color="#555555", fontsize=9, ha="left", transform=top_ax.transAxes)
top_ax.text(1.02, 0.65, "_______________________", fontweight="bold", color="#cccccc", fontsize=9, ha="left", transform=top_ax.transAxes)

# Add label for Global Median line
top_ax.text(global_median, 1.1, "Global Med", color='#34495e', fontsize=9, ha='center', fontweight='bold', transform=top_ax.get_xaxis_transform())

# Adjust spacing between plots
g.figure.subplots_adjust(hspace=-0.35)
g.set_titles("")
g.set(yticks=[], ylabel="")
g.despine(bottom=True, left=True)

# Format X-axis currency
def currency_formatter(x, pos):
    if x >= 1000: return f'₪{int(x/1000)}k'
    return f'₪{int(x)}'

for ax in g.axes.flat:
    ax.xaxis.set_major_formatter(FuncFormatter(currency_formatter))
    ax.set_xlim(0, viz_xlim) # Apply visual zoom
    ax.grid(False)

# Main Titles
plt.suptitle("Top 10 Agents Performance: Deal Size Distribution", y=0.99, fontsize=18, fontweight='bold', color='#1a1a1a')
plt.figtext(0.5, 0.95, "Density normalized per agent", ha="center", fontsize=10, color='#666666')

g.set_xlabels("Order Value (Net)", fontsize=12, fontweight='bold', labelpad=10, color='#555555')

plt.subplots_adjust(left=0.15, right=0.75, top=0.90, bottom=0.1)

plt.show()
```
</details>

<br>

### 📊 Visualization Output (Screenshot)

<div align="center">
  <img src="https://github.com/orelgrBGU/Diplomat_Visualization/blob/main/viz%202.png?raw=true"
       alt="Deal Size Distribution Visualization"
       width="80%"
       style="border: 1px solid #ccc; border-radius: 8px;">
</div>

<br>

## הסבר על הגרף 

הוויזואליזציה חושפת פער אסטרטגי מובהק באופי העבודה של סוכני המכירות. בעוד שהסוכנים המובילים (בראש הגרף, כגון Agent 35 ו-Agent 25) מציגים התפלגות "שטוחה" ורחבה המעידה על תמהיל עסקאות מגוון ונטייה לעסקאות ענק (חציון סביב 40,000₪), הסוכנים בחלק התחתון מתאפיינים בגרף "שפיצי" וצר המעיד על עבודה סיזיפית של מאות עסקאות קטנות וזהות (חציון סביב 9,000₪).



## ויזואליזציה 3 
## מודל WWH – הסבר על הוויזואליזציה

<table dir="rtl">
  <thead>
    <tr>
      <th>רכיב</th>
      <th>תוכן</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>What – מה מוצג?</strong></td>
      <td>
 הגרף מציג מפת חום (Heatmap) של אחוז ההמרה (Conversion Rate) בחלוקה לימי השבוע ולשעות הפעילות (07:00–19:00). כל תא במטריצה מייצג את הסבירות שלקוח שנכנס בשעה וביום מסוימים יבצע רכישה משמעותית (מעל 50 ₪). עוצמת הצבע (מבהיר לכהה) מעידה על גובה אחוז ההמרה, ובנוסף מופיע בתוך כל תא הערך המספרי המדויק באחוזים.
      </td>
    </tr>
    <tr>
      <td><strong>Why – למה בחרנו בגרף הזה?</strong></td>
      <td>
המטרה היא זיהוי דפוסים ומגמות לצורך אופטימיזציה של סידור העבודה. במקום לנחש מתי לשבץ סוכנים, הגרף מראה בבירור מתי העסק נמצא ב"דופק גבוה" (יעילות שיא) ומתי הוא ב"זמן מת". תצוגה זו נבחרה כי היא מונעת את העומס הוויזואלי שהיה נוצר בהצגת גרף קווי עם חמישה קווים חופפים ("ספגטי"), ומאפשרת סריקה הוליסטית ומהירה של כל השבוע במבט אחד.
      </td>
    </tr>
    <tr>
      <td><strong>How – איך הגרף מציג את הנתונים?</strong></td>
      <td>
  הוויזואליזציה משתמשת במיקום מרחבי על גבי גריד (מטריצה): ציר ה-X מייצג את שעות היממה וציר ה-Y את ימי השבוע. המשתנה הכמותי (אחוז ההמרה) מיוצג על ידי ערוץ הצבע (Color Saturation) בסקאלה רציפה של כחולים (תכלת עד כחול עמוק). הנתונים עברו אגרגציה (חישוב ממוצע) לכל שעה ויום, והתווספו תוויות טקסט מספריות לדיוק מקסימלי בקבלת ההחלטות.

   
  
  </tbody>
</table>

<details>
<summary><strong>לחץ להצגת הקוד המלא (Python)</strong></summary>

<br>

```python
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd
import numpy as np
from matplotlib.colors import LinearSegmentedColormap

# --- 1. Data Loading & Preparation ---
# Ensure 'df' is loaded. If running standalone, uncomment:
# df = pd.read_csv('דאטא לויזואליזציה.xlsx - גיליון1.csv')

df.rename(columns={
    'סכום נטו הזמנה ': 'NetAmount',
    'זמן התחלה': 'StartTime',
    'Date': 'Date'
}, inplace=True)

df['Date'] = pd.to_datetime(df['Date'], errors='coerce')
df = df.dropna(subset=['Date'])
df['StartTime'] = pd.to_datetime(df['StartTime'], format='%H:%M:%S', errors='coerce')
df['Hour'] = df['StartTime'].dt.hour
df['DayOfWeek'] = df['Date'].dt.day_name()

# Define Conversion: Orders > 50 NIS
df['IsConversion'] = df['NetAmount'] > 50

# Filter Business Hours (07:00 - 19:00)
df_business = df[(df['Hour'] >= 7) & (df['Hour'] <= 19)].copy()

# Create Pivot Table
heatmap_data = df_business.pivot_table(
    index='DayOfWeek',
    columns='Hour',
    values='IsConversion',
    aggfunc='mean'
) * 100

# Sort Days
days_order = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday']
existing_days = [d for d in days_order if d in heatmap_data.index]
heatmap_data = heatmap_data.reindex(existing_days)

# --- 2. Smart Scaling & NEW Custom Palette ---
# Calculate 5th and 95th percentiles
vmin_smart = np.nanpercentile(heatmap_data.values, 5)
vmax_smart = np.nanpercentile(heatmap_data.values, 95)

# NEW PALETTE: Visible Light Blue -> Deep Navy
# #d1e3f0: Light Blue-Grey (Visible on white paper)
# #08306b: Deep Navy (Strong contrast)
colors = ["#d1e3f0", "#08306b"]
custom_cmap = LinearSegmentedColormap.from_list("custom_navy", colors, N=100)

# --- 3. Plotting ---
plt.figure(figsize=(12, 6))
sns.set_theme(style="white")

ax = sns.heatmap(
    heatmap_data,
    annot=True,
    fmt=".0f",
    cmap=custom_cmap,
    vmin=vmin_smart,
    vmax=vmax_smart,
    linewidths=2,
    linecolor='white',
    cbar_kws={'label': 'Conversion Rate (%)', 'shrink': 0.8}
)

# --- 4. Dynamic Text Color Logic ---
threshold = (vmax_smart + vmin_smart) / 2

for t in ax.texts:
    try:
        val = float(t.get_text())
        if val > threshold:
            t.set_color('white')
            t.set_weight('bold')
        else:
            t.set_color('#1a1a1a') # Almost black for better contrast on light blue
    except ValueError:
        pass

# --- 5. Styling Ticks & Labels ---
ax.tick_params(axis='both', colors='#95a5a6', length=0)
plt.xticks(rotation=0, fontsize=10, fontweight='bold', color='#7f8c8d')
plt.yticks(rotation=0, fontsize=10, fontweight='bold', color='#7f8c8d')

# Axis Titles
ax.set_xlabel("Hour of Day", fontsize=11, fontweight='bold', labelpad=15, color='#7f8c8d')
ax.set_ylabel("", fontsize=11)

# Format X-axis
ax.set_xticklabels([f"{int(h):02d}:00" for h in heatmap_data.columns])

# --- 6. Titles & Footer ---
plt.text(x=0, y=-0.8, s="Conversion rate by day of week and hour of day",
         fontsize=18, fontweight='bold', color='#2c3e50', ha='left')

plt.text(x=0, y=-0.3, s="Retail visits converted to sales above 50 NIS, in percent",
         fontsize=12, color='#555555', ha='left')

plt.figtext(0.5, -0.05,
            "Data reflects average conversion probability based on Q2-Q3 performance. Measured as (Orders > 50 NIS) / (Total Visits).",
            ha="center", fontsize=9, color='#95a5a6')

plt.tight_layout()
plt.show()
```
</details>

<br>

### 📊 Visualization Output (Screenshot)

<div align="center">
  <img src="https://github.com/orelgrBGU/Diplomat_Visualization/blob/main/viz%203.png?raw=true"
       alt="Conversion Rate Heatmap"
       width="85%"
       style="border: 1px solid #ccc; border-radius: 8px;">
</div>

<br>


 ## הסבר על הגרף 

הוויזואליזציה מהווה כלי אבחון אסטרטגי לניהול המשאב היקר ביותר של הארגון – זמן הסוכנים. המפה חושפת את "הדופק העסקי" של השבוע ומבחינה בבירור בין שעות של "מאמץ משתלם" (אזורים כהים עם אחוזי המרה גבוהים) לבין "זמן מת" (אזורים בהירים).

תובנה זו מאפשרת למנהלים לבצע אופטימיזציה של סידור העבודה: במקום לשבץ כוח אדם באופן אחיד, ניתן לתגבר את המשמרות בשעות ה"שיא" שבהן הלקוחות בשלים לקנייה, ולנצל את "החורים הלבנים" (שעות השפל) למשימות אדמיניסטרטיביות, הדרכות או מנוחה, ובכך למקסם את התפוקה מכל שעת עבודה.



# ויזואליזציה 4
## מודל WWH – הסבר על הוויזואליזציה

<table dir="rtl">
  <thead>
    <tr>
      <th>רכיב</th>
      <th>תוכן</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>What – מה מוצג?</strong></td>
      <td>
 הגרף מציג מטריצת פיזור (Scatter Matrix) של 10 הערים המובילות בחברה, הממופות על בסיס שני צירים: משך הביקור הממוצע בדקות (ציר X) וסך ההכנסות המצטבר (ציר Y). כל עיר מיוצגת על ידי סמן בצורת ריבוע, כאשר שטח הריבוע משקף את נפח הפעילות (מספר הביקורים באותה עיר). הרקע מחולק לארבעה אזורי יעילות ("רביעים") בצבעים פסטליים, המסווגים את הערים ל: מצטיינים, טעוני שיפור, ביצועים נמוכים ופוטנציאל לא ממומש.
      </td>
    </tr>
    <tr>
      <td><strong>Why – למה בחרנו בגרף הזה?</strong></td>
      <td>
המטרה העסקית היא לנתח את היעילות התפעולית (ROI על זמן עבודה). מבחינה ויזואלית, הבחירה בריבועים (Squares) במקום בעיגולים קלאסיים נעשתה מתוך שיקול תפיסתי-קוגניטיבי: המחקר מראה שלעין האנושית קל יותר להשוות ולמדוד הבדלי גודל (שטח) בין צורות בעלות קווים ישרים ופינות מאשר בין עיגולים. עיצוב זה מאפשר למנהל לזהות במדויק ערים שבהן מושקעת "מסה" גדולה של ביקורים (ריבועים גדולים) ללא תמורה כספית הולמת.
      </td>
    </tr>
    <tr>
      <td><strong>How – איך הגרף מציג את הנתונים?</strong></td>
      <td>
  הנתונים עברו תהליך ETL שכלל המרה (Parsing) של טווחי שעות טקסטואליים לערכים מספריים (Duration), וסינון חריגים (Outliers). לאחר אגרגציה לפי עיר, הנתונים הוצגו באמצעות ספריית Plotly. הגרף כולל שכבת אינטראקטיביות מתקדמת , נעשה שימוש בצבעים פסטליים רכים להפרדת הרביעים, והוספו שכבות מידע אינטראקטיביות (Tooltips) החושפות מדדי עומק נוספים – כמו "גודל הזמנה ממוצע" ו"יעילות שקלית לדקה" – רק כאשר המשתמש מתמקד בריבוע ספציפי.

   
  
  </tbody>
</table>

<details>
<summary><strong>לחץ להצגת הקוד המלא (Python)</strong></summary>

<br>

```python
import pandas as pd
import plotly.express as px
import plotly.graph_objects as go
import numpy as np

print("--- מתחיל יצירת גרף ריבועים ---")

# ==========================================
# 1. טעינת ועיבוד נתונים (כמו בקוד שעבד לנו)
# ==========================================
if 'df' in locals():
    raw_df = df.copy()
else:
    raise ValueError("❌ לא נמצא משתנה df. טען את הקובץ מחדש.")

# חישוב משך זמן ביקור (מתוך הטקסט "06:29-08:43")
raw_df['Revenue'] = pd.to_numeric(raw_df['Revenue'], errors='coerce').fillna(0)

try:
    time_split = raw_df['זמן ביקור'].astype(str).str.split('-', expand=True)
    start_times = pd.to_datetime(time_split[0], format='%H:%M', errors='coerce')
    end_times = pd.to_datetime(time_split[1], format='%H:%M', errors='coerce')
    raw_df['Duration_Mins'] = (end_times - start_times).dt.total_seconds() / 60
    print("✅ זמנים חושבו בהצלחה.")
except:
    # גיבוי למקרה שהפורמט שונה
    raw_df['Duration_Mins'] = (pd.to_datetime(raw_df['זמן סיום'], errors='coerce') - 
                               pd.to_datetime(raw_df['זמן התחלה'], errors='coerce')).dt.total_seconds() / 60

# סינון
mask = (raw_df['Revenue'] > 0) & (raw_df['Duration_Mins'] > 0) & (raw_df['Duration_Mins'] < 180)
df_plot = raw_df[mask].copy()

# אגרגציה
df_city_level = df_plot.groupby('City').agg({
    'Revenue': 'sum', 
    'Duration_Mins': 'mean', 
    'Date': 'count'
}).reset_index()

# שמות ומדדים
df_city_level.columns = ['City', 'Revenue', 'Duration_Mins', 'Date'] # יישור שמות
df_city_level['Avg_Order'] = df_city_level['Revenue'] / df_city_level['Date']
df_city_level['RPM'] = df_city_level['Revenue'] / (df_city_level['Duration_Mins'] * df_city_level['Date'])

# שמות לעברית
df_city_level = df_city_level.rename(columns={
    'City': 'עיר', 'Revenue': 'סה"כ הכנסות', 'Duration_Mins': 'זמן ביקור ממוצע',
    'Date': 'נפח פעילות (מספר ביקורים)', 'Avg_Order': 'גודל הזמנה ממוצע', 'RPM': 'יעילות תפעולית (₪ לדקה)'
})

# 10 הערים המובילות
df_top10 = df_city_level.sort_values('סה"כ הכנסות', ascending=False).head(10)

# ==========================================
# 2. בניית הגרף (עם ריבועים!)
# ==========================================

avg_time = df_top10['זמן ביקור ממוצע'].mean()
avg_rev = df_top10['סה"כ הכנסות'].mean()

fig = px.scatter(
    df_top10,
    x="זמן ביקור ממוצע",
    y='סה"כ הכנסות',
    size="נפח פעילות (מספר ביקורים)", # גודל הריבוע
    color="עיר",
    text="עיר",
    hover_data={"עיר": False, "סה\"כ הכנסות": ':,.0f', "זמן ביקור ממוצע": ':.1f', "נפח פעילות (מספר ביקורים)": True},
    title="מטריצת ביצועים אסטרטגית: ניתוח יעילות ערים",
    template="plotly_white",
    height=750
)

# --- השינוי המרכזי: הפיכת העיגולים לריבועים ---
fig.update_traces(
    marker_symbol='square',  # <=== זה מה שהופך לריבועים
    textposition='top center', 
    textfont_weight="bold", 
    marker=dict(line=dict(width=1.5, color='white'), opacity=0.9)
)

# ==========================================
# 3. עיצוב רקעים ותוויות
# ==========================================
x_min, x_max = df_top10['זמן ביקור ממוצע'].min() * 0.9, df_top10['זמן ביקור ממוצע'].max() * 1.1
y_min, y_max = df_top10['סה"כ הכנסות'].min() * 0.9, df_top10['סה"כ הכנסות'].max() * 1.1

# רקעים פסטליים
fig.add_shape(type="rect", x0=x_min, y0=avg_rev, x1=avg_time, y1=y_max, fillcolor="#D4EFDF", opacity=0.5, layer="below", line_width=0)
fig.add_shape(type="rect", x0=avg_time, y0=y_min, x1=x_max, y1=avg_rev, fillcolor="#FADBD8", opacity=0.5, layer="below", line_width=0)
fig.add_shape(type="rect", x0=avg_time, y0=avg_rev, x1=x_max, y1=y_max, fillcolor="#FAE5D3", opacity=0.5, layer="below", line_width=0)
fig.add_shape(type="rect", x0=x_min, y0=y_min, x1=avg_time, y1=avg_rev, fillcolor="#D6EAF8", opacity=0.5, layer="below", line_width=0)

# קווים לבנים
fig.add_vline(x=avg_time, line_dash="solid", line_color="white", line_width=3)
fig.add_hline(y=avg_rev, line_dash="solid", line_color="white", line_width=3)

# תוויות בפינות
def add_label(x, y, text, color, align, x_shift, y_shift):
    fig.add_annotation(x=x, y=y, text=f"<b>{text}</b>", showarrow=False, font=dict(size=14, color=color, family="Arial Black"), bgcolor="rgba(255,255,255,0.6)", xanchor=align, xshift=x_shift, yshift=y_shift)

add_label(x_min, y_max, "💎 מצטיינים", "#196F3D", "left", 10, -10)
add_label(x_max, y_min, "⚠️ ביצועים נמוכים", "#943126", "right", -10, 10)
add_label(x_max, y_max, "🔨 דורש התייעלות", "#AF601A", "right", -10, -10)
add_label(x_min, y_min, "🚀 פוטנציאל", "#2874A6", "left", 10, 10)

fig.update_layout(
    showlegend=False, 
    margin=dict(t=90, b=60, l=60, r=60), 
    xaxis=dict(title="<b>משך ביקור ממוצע (דקות)</b> ", range=[x_min, x_max]),
    yaxis=dict(title="<b>סה\"כ הכנסות (₪)</b>", range=[y_min, y_max])
)

# שמירה
try:
    fig.write_image("Strategic_Matrix_Squares.png", scale=3, width=1200, height=800)
    print("✅ תמונה נשמרה: Strategic_Matrix_Squares.png")
except:
    print("⚠️ לא ניתן לשמור תמונה אוטומטית.")

fig.show()
```
</details>

<br>

### 📊 Visualization Output (Screenshot)

<div align="center">
  <img src="https://github.com/orelgrBGU/Diplomat_Visualization/blob/main/Strategic_Matrix_Squares.png?raw=true"
       alt="Strategic Efficiency Matrix"
       width="85%"
       style="border: 1px solid #ccc; border-radius: 8px;">
</div>


<br>

## הסבר על הגרף

הויזואליזציה מאפשרת לנו לראות שהערים המובילות (ברביע הירוק) אינן מתאפיינות רק בהכנסות גבוהות, אלא גם בביקורים קצרים וממוקדים – מה שמעיד על תהליך מכירה "חד" ויעיל. לעומת זאת, ככל שזזים ימינה במטריצה (לכיוון האדום/כתום), הגרף ממחיש "בזבוז משאבים": הריבועים נשארים גדולים (נפח פעילות גבוה), אך נמתחים על פני זמן רב מדי ללא עלייה תואמת בהכנסה. מה שמעיד כנראה על עיכובים לוגיסטיים או "זמן מת" שבו הסוכן ממתין בסניף ללא מעש.
