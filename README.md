
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
      <td><strong>What</strong></td>
      <td>
 הגרף מציג את התפלגות הביקורים שבוצעו בפועל אצל לקוחות במהלך היום, בין השעות 07:00 ל־19:00. לכל ביקור חישבנו את משך הזמן בדקות,סיווגנו כל ביקור לשלוש קטגוריות זמן: ביקור קצר מאוד (“Touch & Go” – עד 10 דקות), ביקור סטנדרטי יעיל (10–45 דקות) וביקור ארוך או תקוע (מעל 45 דקות). בגרף רואים עבור כל שעה כמה ביקורים התרחשו, וכמה מהם שייכים לכל אחת משלוש הקטגוריות הללו.
      </td>
    </tr>
    <tr>
      <td><strong>Why</strong></td>
      <td>
הגרף מאפשר לזהות באילו שעות היום יש נפח ביקורים גבוה במיוחד, האם בשעות השיא יש בעיקר ביקורים קצרים ויעילים או דווקא הרבה ביקורים ארוכים, והאם יש חלונות זמן שבהם הסוכנים “נתקעים” אצל לקוחות על חשבון לקוחות אחרים ויכול לאפשר כמשוב לניהול זמן נכון יותר.
      </td>
    </tr>
    <tr>
      <td><strong>How</strong></td>
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

#  Data Preprocessing

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

# Categorization Logic 
def classify_duration(mins):
    if mins <= 10:
        return '1. Touch & Go (<10m)'      # Short visits
    elif mins <= 45:
        return '2. Standard Work (10-45m)' # Effective time
    else:
        return '3. Deep/Stuck (>45m)'      # Long visits

df_visits['Duration_Category'] = df_visits['duration_mins'].apply(classify_duration)

# Visualization
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

###  Visualization Output 

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
      <td><strong>What</strong></td>
      <td>
הנתונים כוללים רשומות של עסקאות שבוצעו על ידי סוכנים שונים. כל רשומה מכילה מזהה סוכן, ערך כספי של העסקה בשקלים, ומידע נגזר כגון מספר העסקאות הכולל לכל סוכן וחציון ערכי העסקאות שלו. הנתונים עוברים אגרגציה כך שלכל סוכן מתקבלת התפלגות של סכומי עסקאות, ולא רשימת עסקאות גולמית. הסדר בציר האנכי נקבע לפי ערך החציון של כל סוכן, ללא פרשנות עסקית, אלא כמאפיין מבני של הנתונים בלבד
      </td>
    </tr>
    <tr>
      <td><strong>Why</strong></td>
      <td>
המטרה היא להבין איך כל אחד מעשרת הסוכנים המובילים מוכר בפועל ולא רק כמה הוא מכר בסך הכול. הגרף מאפשר לזהות את דפוס ההתנהלות של כל סוכן ולבחון האם הוא נשען על מעט עסקאות גדולות או על נפח גבוה של עסקאות קטנות. כך ניתן לחשוף את ״אישיות המכירה״ של כל סוכן ולא רק את השורה התחתונה שלו. ההשוואה מתבצעת דרך הצורה, הפיזור והמיקום היחסי של ההתפלגויות, ולא דרך ערך בודד. הבחירה בתצוגה זו מאפשרת השוואה אנכית ברורה בין סוכנים ומונעת עומס חזותי שהיה נוצר מהצגת היסטוגרמות נפרדות.
      </td>
    </tr>
    <tr>
      <td><strong>How</strong></td>
      <td>
 הוויזואליזציה ממומשת כRidge Plot שבו ציר ה־X מייצג ערכים כספיים רציפים לאחר סינון עסקאות קטנות וחיתוך קיצונים, והציר האנכי מחלק את הנתונים לשורות נפרדות לפי סוכן. כל רצועה מציגה התפלגות צפיפות של סכומי העסקאות באמצעות שטח רציף, המאפשר קריאה חלקה של הצורה והפיזור. החפיפה המבוקרת בין הרצועות מצמצמת עומס ויזואלי תוך שמירה על השוואה ישירה. קו ייחוס גלובלי נוסף כעוגן קבוע להשוואה בין כל הסוכנים. המבנה כולו נועד לאפשר קריאה מהירה של הבדלים מבניים בהתפלגות ולא זיהוי של ערכים נקודתיים.
   
  
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

### Visualization Output

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
      <td><strong>What</strong></td>
      <td>
הנתונים מייצגים שיעורי המרה מחושבים עבור שילובים של יום בשבוע ושעת פעילות. כל תא מייצג ערך כמותי אחד ,אחוז ההמרה הממוצע באותו יום ובאותה שעה (לאחר סינון עסקאות שאינן עומדות בסף מינימלי). מבנה הנתונים הוא טבלאי, דו-ממדי, עם שני משתנים קטגוריאליים (יום, שעה) ומשתנה כמותי אחד (אחוז המרה). אין כאן רצף אירועים או ישויות נפרדות, אלא סיכום סטטיסטי של פעילות לאורך זמן.
      </td>
    </tr>
    <tr>
      <td><strong>Why</strong></td>
      <td>
המטרה היא זיהוי דפוסים ומגמות לצורך אופטימיזציה של סידור העבודה ובנוסף לזהות דפוסים זמניים בהתנהגות הלקוחות ולהבין מתי מתרחשת פעילות אפקטיבית יותר או פחות. במקום לנחש מתי לשבץ סוכנים, הגרף מראה בבירור מתי העסק נמצא ביעילות שיא ומתי הוא ב"זמן מת".  
המוטיבציה לתת להנהלה יכולת להשוות בין חלונות זמן שונים כדי לאתר שעות וימים בעלי פוטנציאל גבוה או נמוך לביצועי מכירה. הדגש הוא על השוואה רוחבית והבנת מבנה הפעילות לאורך השבוע, ולא על ניתוח נקודתי של אירוע בודד.
      </td>
    </tr>
    <tr>
      <td><strong>How</strong></td>
      <td>
 הנתונים מיוצגים באמצעות מפת חום דו־ממדית. הציר האופקי מקודד את ממד הזמן לפי שעות היום, והציר האנכי מקודד את ימי השבוע. כל תא במטריצה מייצג ערך יחיד של שיעור ההמרה, המקודד באמצעות ערוץ צבע רציף. עוצמת הצבע משקפת את גובה הערך הכמותי, ללא שימוש בגודל, צורה או סימבול נוסף. הנתונים עברו אגרגציה לפי צמד (יום, שעה), והערך המספרי מוצג בתוך התא כתווית טקסטואלית משלימה. המבנה הגרידי מאפשר השוואה ישירה בין תאים סמוכים הן אופקית והן אנכית, ללא חפיפה או קווי חיבור..

   
  
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

#  Data Loading & Preparation 
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

#  Scaling & NEW Custom Palette 
# Calculate 5th and 95th percentiles
vmin_smart = np.nanpercentile(heatmap_data.values, 5)
vmax_smart = np.nanpercentile(heatmap_data.values, 95)


# #08306b: Deep Navy (Strong contrast)
colors = ["#d1e3f0", "#08306b"]
custom_cmap = LinearSegmentedColormap.from_list("custom_navy", colors, N=100)

#  Plotting 
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

# Dynamic Text Color Logic 
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

#  Styling Ticks & Labels 
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

###  Visualization Output 

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
      <td><strong>What </strong></td>
      <td>
 הוויזואליזציה מציגה Diverging Bar Chart (תרשים עמודות מתפצל) הממפה את איכות הניהול התפעולי של מנהלי הסוכנים. כל שורה מייצגת מנהל, והנתונים מנורמלים ל-100% פעילות. הציר המרכזי (האפס) מפריד בין שני עולמות: צד ימין (ירוק) מייצג ביקורים תקינים (שתוכננו ובוצעו), וצד שמאל (אדום/כתום) מייצג חריגות (ביקורים לא מתוכננים או שלא בוצעו כנדרש). בנוסף, כל צד מפוצל פנימית לפי ערוץ הפעילות: פיזי מול טלפוני.
      </td>
    </tr>
    <tr>
      <td><strong>Why </strong></td>
      <td>
ההמטרה העסקית היא לעבור ממדידת "כמות" למדידת "איכות ומשמעת". גרף עמודות רגיל היה מקשה להשוות את היחס בין תכנון לביצוע. הבחירה בגרף מתפצל (Diverging) היא אסטרטגית: היא מאפשרת למקבל ההחלטות לראות בבת-אחת את "המאזן" של כל מנהל. העין תופסת מיידית מי "ירוק" (ממושמע) ומי "אדום" (פועל ללא תכנון), ומונעת מהמספרים המוחלטים להסתיר בעיות התנהגותיות.
      </td>
    </tr>
    <tr>
      <td><strong>How</strong></td>
      <td>
  הנתונים עברו אגרגציה וחישוב אחוזים יחסיים לכל מנהל. נעשה שימוש בקידוד צבע כפול: גוון (Hue) להפרדה בין טוב (ירוק) לרע (אדום), ובהירות (Lightness) להבחנה בין סוגי המדיה (פיזי/טלפוני). הטכניקה הוויזואלית נקראת Relative Stacking, המאפשרת השוואה הוגנת בין מנהלים ללא תלות בנפח הפעילות הכולל שלהם. האינטראקטיביות (Hover) חושפת את האחוזים המדויקים בכל פלח.

   
  
  </tbody>
</table>

<details>
<summary><strong>לחץ להצגת הקוד המלא (Python)</strong></summary>

<br>

```python
import pandas as pd
import plotly.graph_objects as go
import io


# Load File

try:
    from google.colab import files
    uploaded = files.upload()
    filename = next(iter(uploaded))
    file_bytes = uploaded[filename]

    try:
        df = pd.read_csv(io.BytesIO(file_bytes))
    except:
        df = pd.read_excel(io.BytesIO(file_bytes))

except ImportError:
    file_path = input("Enter full path to CSV or Excel file: ")
    try:
        df = pd.read_csv(file_path)
    except:
        df = pd.read_excel(file_path)

print("File loaded successfully")

#  Rename & Clean Columns

df = df.rename(columns={
    'מנהל סוכן ': 'Manager',
    'האם תוכנן': 'Planned',
    'האם תוכנן ובוצע': 'PlannedExecuted',
    'האם ביקר בפועל': 'Visited',
    'סוג ביקור': 'VisitType'
})

# Normalize VisitType (fix spelling + casing)
df['VisitType'] = (
    df['VisitType']
    .astype(str)
    .str.strip()
    .replace({
        'Fisical': 'Physical',
        'fisical': 'Physical',
        'Physical': 'Physical',
        'Phone': 'Phone',
        'phone': 'Phone'
    })
)

df = df[
    df['Planned'].isin([0, 1]) &
    df['PlannedExecuted'].isin([0, 1]) &
    df['Visited'].isin([0, 1]) &
    df['VisitType'].isin(['Physical', 'Phone'])
].copy()

# Classification Logic

def classify(row):
    # Planned and executed
    if row['Planned'] == 1 and row['PlannedExecuted'] == 1 and row['Visited'] == 1:
        return f"Planned & Executed – {row['VisitType']}"

    # Unplanned but happened
    if row['Planned'] == 0 and row['PlannedExecuted'] == 0 and row['Visited'] == 1:
        return f"Not Compliant – {row['VisitType']}"

    # Planned but not executed
    if row['Planned'] == 1 and row['PlannedExecuted'] == 0 and row['Visited'] == 0:
        return f"Not Compliant – {row['VisitType']}"

    return None

df['Category'] = df.apply(classify, axis=1)
df = df[df['Category'].notna()]

# Distribution per Manager (Percent)

counts = (
    df
    .groupby(['Manager', 'Category'])
    .size()
    .unstack(fill_value=0)
)

dist = counts.div(counts.sum(axis=1), axis=0) * 100

cols = [
    'Not Compliant – Physical',
    'Not Compliant – Phone',
    'Planned & Executed – Physical',
    'Planned & Executed – Phone'
]

for c in cols:
    if c not in dist.columns:
        dist[c] = 0

dist = dist[cols]
managers = dist.index.tolist()

#  Plotly Diverging Bar Chart

fig = go.Figure()

# Left side – Not Compliant
fig.add_bar(
    y=managers,
    x=-dist['Not Compliant – Physical'],
    name='Not Compliant – Physical',
    orientation='h',
    marker_color='#d73027',
    customdata=dist['Not Compliant – Physical'],
    hovertemplate='Not Compliant – Physical<br>Share: %{customdata:.1f}%<extra></extra>'
)

fig.add_bar(
    y=managers,
    x=-dist['Not Compliant – Phone'],
    name='Not Compliant – Phone',
    orientation='h',
    marker_color='#fc8d59',
    customdata=dist['Not Compliant – Phone'],
    hovertemplate='Not Compliant – Phone<br>Share: %{customdata:.1f}%<extra></extra>'
)

# Right side – Planned & Executed
fig.add_bar(
    y=managers,
    x=dist['Planned & Executed – Physical'],
    name='Planned & Executed – Physical',
    orientation='h',
    marker_color='#1a9850',
    hovertemplate='Planned & Executed – Physical<br>Share: %{x:.1f}%<extra></extra>'
)

fig.add_bar(
    y=managers,
    x=dist['Planned & Executed – Phone'],
    name='Planned & Executed – Phone',
    orientation='h',
    marker_color='#66bd63',
    hovertemplate='Planned & Executed – Phone<br>Share: %{x:.1f}%<extra></extra>'
)

fig.update_layout(
    barmode='relative',
    title=dict(
        text='Planning and Execution Discipline by Manager<br><sup>Split by Visit Type</sup>',
        x=0.5
    ),
    xaxis=dict(
        title='Percentage of Visits',
        range=[-100, 100],
        tickvals=[-100, -75, -50, -25, 0, 25, 50, 75, 100],
        ticktext=['100', '75', '50', '25', '0', '25', '50', '75', '100'],
        zeroline=True,
        zerolinewidth=2
    ),
    yaxis_title='Manager',
    legend_title='Category',
    template='plotly_white',
    height=650
)

fig.show()

#  Export to HTML + Download

html_file = "planning_execution_discipline_by_manager.html"

fig.write_html(
    html_file,
    config={
        "scrollZoom": True,
        "displayModeBar": True
    }
)

try:
    from google.colab import files
    files.download(html_file)
except:
    pass

```
</details>

<br>

### Visualization Output


<div align="center">
  <img src="https://github.com/orelgrBGU/Diplomat_Visualization/blob/main/newplot.png?raw=true"
       alt="Planning Discipline Visualization"
       width="85%"
       style="border: 1px solid #ccc; border-radius: 8px;">

  <br><br>
  
  <a href="https://htmlpreview.github.io/?https://github.com/orelgrBGU/Diplomat_Visualization/blob/main/planning_discipline.html" target="_blank">
    <img src="https://img.shields.io/badge/VIEW_INTERACTIVE_GRAPH-Click_Here-brightgreen?style=for-the-badge&logo=html5&logoColor=white" alt="View Interactive Graph">
  </a>
  
  <p style="font-size: 14px; color: #555;">
    👆 <b>לחץ על הכפתור הירוק כדי לשחק עם הנתונים בזמן אמת</b>
  </p>
</div>
<br>

## הסבר על הגרף

הויזואליזציה מציגה את מדד "משמעת הביצוע" של המנהלים, כשהיא מחלקת את הפעילות לשני עולמות: צד ימין (הירוק) משקף עבודה תקינה שבוצעה בדיוק לפי התכנון, בעוד צד שמאל (האדום/כתום) חושף חריגות ועבודה לא מתוכננת.
ניתן לראות בבירור דפוס מעניין: רוב החריגות והעבודה הלא-מתוכננת (בצד השמאלי) מתבצעות בטלפון (הגוונים הבהירים), בעוד שביקורים פיזיים נוטים להיות מתוכננים ומוקפדים יותר. הגרף מאפשר להנהלה לזהות במבט אחד מי מהמנהלים עובד בצורה מסודרת ושיטתית, ומי פועל בצורה ריאקטיבית של "כיבוי שריפות" ועיגול פינות מרחוק.



# ויזואליזציה 5
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
      <td><strong>What</strong></td>
      <td>
 הוויזואליזציה מציגה מפת חום גאוגרפית (Density Map) הממפה את היקף המכירות המצטבר בכל עיר בישראל. הנתונים מבוססים על קואורדינטות (Latitude/Longitude) של כל עיר, כאשר "עוצמת החום" (הצבע והבהירות) מייצגת את סך המכירות במיליוני שקלים. המפה משתמשת בסקאלת צבעים רציפה הנעה מצהוב (פעילות נמוכה) לאדום כהה (מוקדי כוח).
      </td>
    </tr>
    <tr>
      <td><strong>Why</strong></td>
      <td>
המטרה העסקית היא לזהות דפוסים מרחביים שקשה לראות בטבלאות אקסל רגילות. טבלה ממיינת ערים לפי שם או סכום, אך מנתקת אותן מההקשר הגיאוגרפי שלהן. מפת החום נבחרה כי היא מאפשרת למנהלים לזהות במבט אחד "כתמי נפט" של הצלחה (אזורים שבהם אנו שולטים בשוק) לעומת אזורים שבהם הפעילות דלילה מדי, ובכך לייעל את מערך ההפצה והלוגיסטיקה.
      </td>
    </tr>
    <tr>
      <td><strong>How</strong></td>
      <td>
  התהליך כלל שלב Geocoding (המרה של שמות ערים לקואורדינטות GPS) באמצעות ספריית geopy. הנתונים הוצגו על גבי תשתית המפות של Mapbox בסגנון "Dark Matter" (רקע כהה), בחירה עיצובית שמבליטה את נקודות הצבע הזוהרות ומקלה על זיהוי מוקדים. האינטראקטיביות מאפשרת למשתמש לבצע Zoom-in לרמת הרחוב, ולרחף עם העכבר כדי לראות נתוני עומק מדוייקים לכל עיר (כמות הזמנות, סך קרטונים, ומכירות נטו).

   
  
  </tbody>
</table>

<details>
<summary><strong>לחץ להצגת הקוד המלא (Python)</strong></summary>

<br>

```python
import pandas as pd
import plotly.express as px
import io
import os
from geopy.geocoders import Nominatim
from geopy.extra.rate_limiter import RateLimiter
from google.colab import files

# =========================
# 1. Load File
# =========================

uploaded = files.upload()
filename = next(iter(uploaded))
file_bytes = uploaded[filename]

try:
    df = pd.read_csv(io.BytesIO(file_bytes))
except:
    df = pd.read_excel(io.BytesIO(file_bytes))


#  Data Preparation
df = df.rename(columns={
    'עיר': 'city',
    'סכום נטו הזמנה ': 'NetAmount',
    'סהכ קרטונים בהזמנה': 'TotalCartons'
})

df = df[
    df['city'].notna() &
    (df['NetAmount'] > 0)
].copy()

city_agg = (
    df
    .groupby('city', as_index=False)
    .agg(
        TOTAL_ORDERS=('NetAmount', 'count'),
        TOTAL_SALES=('NetAmount', 'sum'),
        TOTAL_CARTONS=('TotalCartons', 'sum')
    )
)

city_agg['SALES_M'] = city_agg['TOTAL_SALES'] / 1_000_000

#  Geocoding with Cache

coords_cache_path = "city_coords_cache_sales.csv"

if os.path.exists(coords_cache_path):
    coords_cache = pd.read_csv(coords_cache_path)
else:
    coords_cache = pd.DataFrame(columns=["city", "lat", "lon"])

city_agg = city_agg.merge(coords_cache, on="city", how="left")

geolocator = Nominatim(user_agent="sales_heatmap_israel")
geocode = RateLimiter(geolocator.geocode, min_delay_seconds=1)

for idx, row in city_agg[city_agg["lat"].isna()].iterrows():
    location = geocode(f"{row['city']}, Israel")
    if location:
        city_agg.at[idx, "lat"] = location.latitude
        city_agg.at[idx, "lon"] = location.longitude
        print(f"Geocoded {row['city']}")
    else:
        print(f"Skipped {row['city']}")

city_agg[["city", "lat", "lon"]].dropna().to_csv(
    coords_cache_path, index=False
)

city_agg = city_agg.dropna(subset=["lat", "lon"])

#  Map Visualization 
fig = px.density_mapbox(
    city_agg,
    lat="lat",
    lon="lon",
    z="SALES_M",
    radius=35,
    center=dict(lat=31.5, lon=34.8),
    zoom=6,
    mapbox_style="carto-darkmatter",
    color_continuous_scale="YlOrRd",
    hover_name="city",
    hover_data={
        "TOTAL_ORDERS": True,
        "TOTAL_SALES": True,
        "TOTAL_CARTONS": True,
        "SALES_M": True
    },
    title="Sales Heatmap by City"
)

fig.update_traces(
    hovertemplate=
    "<b>%{hovertext}</b><br><br>"
    "Sales (Million ₪): %{z:.2f}<br>"
    "Total Orders: %{customdata[0]}<br>"
    "Total Net Sales (₪): %{customdata[1]:,.0f}<br>"
    "Total Cartons: %{customdata[2]}<extra></extra>"
)

fig.update_layout(
    title=dict(
        text="Sales Heatmap by City",
        x=0.5,
        xanchor="center"
    )
)

fig.show(
    config={
        "scrollZoom": True,
        "displayModeBar": True
    }
)

# Export to HTML

html_file = "sales_heatmap_by_city.html"

fig.write_html(
    html_file,
    config={
        "scrollZoom": True,
        "displayModeBar": True
    }
)

files.download(html_file)

```
</details>

<br>

###  Visualization Output 


<div align="center">
  <img src="https://github.com/orelgrBGU/Diplomat_Visualization/blob/main/newplot%20(3).png?raw=true"
       alt="Sales Heatmap Visualization"
       width="85%"
       style="border: 1px solid #ccc; border-radius: 8px;">

  <br><br>
  
  <a href="https://htmlpreview.github.io/?https://github.com/orelgrBGU/Diplomat_Visualization/blob/main/sales_heatmap_by_city.html" target="_blank">
    <img src="https://img.shields.io/badge/VIEW_INTERACTIVE_GRAPH-Click_Here-brightgreen?style=for-the-badge&logo=html5&logoColor=white" alt="View Interactive Graph">
  </a>
  
  <p style="font-size: 14px; color: #555;">
    👆 <b>לחץ על הכפתור הירוק כדי לשחק עם הנתונים בזמן אמת</b>
  </p>
</div>

<br>

## הסבר על הגרף

התרשים מציג את התפלגות המכירות הארצית, כאשר עוצמת הצבע מעידה על נפח הפעילות הכספי. ניתן לראות בבירור שהליבה העסקית מרוכזת במרכז הארץ, היוצרת "כתם חום" גדול ורציף. לעומת זאת, באזורי הצפון והדרום הפעילות מבוזרת יותר ומתרכזת בערים בודדות בלבד. תצוגה זו מאפשרת למקבלי ההחלטות לזהות פערים לוגיסטיים ולבחון האם ישנם אזורים גיאוגרפיים שלמים ש"נזנחו" או שאינם מקבלים כיסוי מספק מצוותי המכירות.




# ויזואליזציה 6
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
      <td><strong>What</strong></td>
      <td>
 הנתונים מבוססים על רשומות תפעוליות שעברו אגרגציה (Aggregation) לרמת העיר, כך שכל פריט  מייצג סיכום פעילות גיאוגרפי ולא ביקור בודד. כל רשומה כוללת משתנה קטגוריאלי לזיהוי (שם העיר) ושלושה משתנים כמותיים: משך ביקור ממוצע (רציף), סך הכנסות (רציף), ומספר הביקורים. הטבלה מייצגת "תמונת מצב" סטטיסטית של היעילות התפעולית בערים המובילות.
    <tr>
      <td><strong>Why</strong></td>
      <td>
הוויזואליזציה מאפשרת למנהלים לזהות מתאמים (Correlations) בין השקעת המשאבים (זמן הסוכן) לבין התוצאה העסקית הכנסות כסף לחברה בפועל בסופו של דבר, ולאתר חריגים (Outliers) – ערים שבהן זמן הביקור קצר אך ההכנסה גבוהה  שהם מייצגים הצטיינות, או להפך הכנסות נמוכות ובזבוז זמן יקר של סוכנים בסניפים. הגרף מציג את "פרופיל היעילות" של העיר: האם ההכנסות הגבוהות נובעות מביקורים קצרים וממוקדים, או שהן דורשות זמן רב.
      </td>
    </tr>
    <tr>
      <td><strong>How</strong></td>
      <td>
 הנתונים מיוצגים באמצעות תרשים בועות (Bubble Chart), המהווה הרחבה של תרשים פיזור (Scatter Plot). שני המשתנים הרציפים מקודדים באמצעות מיקום מרחבי על גבי מערכת צירים משותפת: ציר ה-X מקודד את "ההשקעה" (זמן ביקור ממוצע), וציר ה-Y מקודד את "התפוקה" (סך הכנסות). המשתנה השלישי, נפח הפעילות, מקודד באמצעות ערוץ הגודל (Size/Area) של הסימן הגרפי, אשר עוצב כריבוע (Square Mark) כדי להבדיל בין גדלים בצורה יותר מעיגול לפי מה שלמדנו בהרצאות. השימוש בערוץ הצבע (Color Hue) הוא קטגוריאלי ומשמש לזיהוי (Identity) של הערים השונות.

   
  
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

# ==========================================
# 1. עיבוד נתונים (Data Processing)
# ==========================================

if 'df' in locals():
    raw_df = df.copy()
else:
    print("Warning: 'df' not found. Please load your data first.")

# ניקוי הכנסות
raw_df['Revenue'] = pd.to_numeric(raw_df['Revenue'], errors='coerce').fillna(0)

# חישוב משך זמן (Duration)
try:
    time_split = raw_df['זמן ביקור'].astype(str).str.split('-', expand=True)
    start_times = pd.to_datetime(time_split[0], format='%H:%M', errors='coerce')
    end_times = pd.to_datetime(time_split[1], format='%H:%M', errors='coerce')
    raw_df['Duration_Mins'] = (end_times - start_times).dt.total_seconds() / 60
except:
    raw_df['Duration_Mins'] = (pd.to_datetime(raw_df['זמן סיום'], errors='coerce') - 
                               pd.to_datetime(raw_df['זמן התחלה'], errors='coerce')).dt.total_seconds() / 60

# סינון נתונים תקינים
mask = (raw_df['Revenue'] > 0) & (raw_df['Duration_Mins'] > 0) & (raw_df['Duration_Mins'] < 180)
df_plot = raw_df[mask].copy()

# אגרגציה לפי עיר
df_city_level = df_plot.groupby('City').agg({
    'Revenue': 'sum', 
    'Duration_Mins': 'mean', 
    'Date': 'count'
}).reset_index()

# הסרת רווחים מיותרים
df_city_level['City'] = df_city_level['City'].astype(str).str.strip()

# ==========================================
# 2. תרגום ועיבוד שמות (English Translation)
# ==========================================

city_map = {
    'ירושלים': 'Jerusalem',
    'תל אביב - יפו': 'Tel Aviv',
    'תל אביב': 'Tel Aviv',
    'תל-אביב': 'Tel Aviv',
    'חיפה': 'Haifa',
    'ראשון לציון': 'Rishon LeTsiyon',
    'פתח תקווה': 'Petah Tikva',
    'פתח-תקווה': 'Petah Tikva',
    'אשדוד': 'Ashdod',
    'נתניה': 'Netanya',
    'באר שבע': 'Beersheba',
    'בני ברק': 'Bnei Brak',
    'חולון': 'Holon',
    'רמת גן': 'Ramat Gan',
    'אשקלון': 'Ashkelon',
    'רחובות': 'Rehovot',
    'בת ים': 'Bat Yam',
    'בית שמש': 'Beit Shemesh',
    'כפר סבא': 'Kfar Saba',
    'הרצליה': 'Herzliya',
    'חדרה': 'Hadera',
    'מודיעין': 'Modiin',
    'מודיעין מכבים רעות': 'Modiin',
    'מודיעים מכבים רעות': 'Modiin',
    'מודיעין-מכבים-רעות': 'Modiin',
    'נצרת': 'Nazareth',
    'לוד': 'Lod',
    'רמלה': 'Ramla',
    'רעננה': 'Ra\'anana',
    'גבעתיים': 'Givatayim',
    'הוד השרון': 'Hod HaSharon',
    'קריית אתא': 'Kiryat Ata',
    'נהריה': 'Nahariya',
    'אילת': 'Eilat'
}

df_city_level['City'] = df_city_level['City'].map(city_map).fillna(df_city_level['City'])

# שינוי שמות עמודות לאנגלית
df_city_level = df_city_level.rename(columns={
    'Revenue': 'Total Revenue',
    'Duration_Mins': 'Avg Visit Duration',
    'Date': 'Visit Count'
})

df_top10 = df_city_level.sort_values('Total Revenue', ascending=False).head(10)

# ==========================================
# 3. בניית הגרף (Clean & Interactive)
# ==========================================

fig = px.scatter(
    df_top10,
    x="Avg Visit Duration",
    y="Total Revenue",
    size="Visit Count",
    color="City",
    
    # תיקון האינטראקטיביות (Hover)
    hover_name="City",
    hover_data={
        "City": False,
        "Total Revenue": ':,.0f',
        "Avg Visit Duration": ':.1f',
        "Visit Count": True
    },
    
    text="City",
    title="City Efficiency Analysis: Revenue vs. Time",
    template="plotly_white",
    height=700
)

# עיצוב הסמנים (ריבועים)
fig.update_traces(
    marker_symbol='square',
    textposition='top center', 
    textfont=dict(size=12, family="Arial", color="black"),
    marker=dict(line=dict(width=1, color='DarkSlateGrey'), opacity=0.8)
)

fig.update_layout(
    showlegend=False,
    margin=dict(t=80, b=50, l=50, r=50),
    xaxis=dict(
        title="<b>Avg Visit Duration (Minutes)</b>",
        showgrid=True,
        gridcolor='#f0f0f0'
    ),
    yaxis=dict(
        title="<b>Total Revenue (NIS)</b>",
        showgrid=True,
        gridcolor='#f0f0f0'
    ),
    title=dict(font=dict(size=24))
)

# ==========================================
# 4. הוספת המקרא (Legend) בפינה הימנית העליונה
# ==========================================

fig.add_annotation(
    x=0.99, y=0.98,          # מיקום: פינה ימנית עליונה
    xref="paper", yref="paper",
    text="<b>Legend:</b><br>■ Square Size = <b>Visit Count</b>", # הטקסט במקרא
    showarrow=False,
    align="left",
    font=dict(size=13, color="black"),
    
    # עיצוב הקופסה (כמו מקרא רגיל)
    bgcolor="rgba(255, 255, 255, 0.9)", 
    bordercolor="#333", 
    borderwidth=1,
    borderpad=8
)

# ==========================================
# 5. שמירה
# ==========================================

fig.write_image("Clean_City_Matrix_Final.png", scale=3, width=1200, height=800)
fig.write_html("clean_ciגדגדגדגדגדגדגדגדty_matrix_final.html")

fig.show()
```
</details>

<br>

### Visualization Output

<div align="center">
  <img src="https://github.com/orelgrBGU/Diplomat_Visualization/blob/main/FIX%20PNG.png?raw=true"
       alt="Strategic Efficiency Matrix"
       width="85%"
       style="border: 1px solid #ccc; border-radius: 8px;">

  <br><br>
  
  <a href="https://htmlpreview.github.io/?https://github.com/orelgrBGU/Diplomat_Visualization/blob/main/FIX%20HTML.html" target="_blank">
    <img src="https://img.shields.io/badge/VIEW_INTERACTIVE_GRAPH-Click_Here-brightgreen?style=for-the-badge&logo=html5&logoColor=white" alt="View Interactive Graph">
  </a>
  
  <p style="font-size: 14px; color: #555;">
    👆 <b>לחץ על הכפתור הירוק כדי לשחק עם הנתונים בזמן אמת</b>
  </p>
</div>
<br>

## הסבר על הגרף

הויזואליזציה מאפשרת לנו לראות שהערים המובילות (ברביע הירוק) אינן מתאפיינות רק בהכנסות גבוהות, אלא גם בביקורים קצרים וממוקדים – מה שמעיד על תהליך מכירה "חד" ויעיל. לעומת זאת, ככל שזזים ימינה במטריצה (לכיוון האדום/כתום), הגרף ממחיש "בזבוז משאבים": הריבועים נשארים גדולים (נפח פעילות גבוה), אך נמתחים על פני זמן רב מדי ללא עלייה תואמת בהכנסה. מה שמעיד כנראה על עיכובים לוגיסטיים או "זמן מת" שבו הסוכן ממתין בסניף ללא מעש.


