
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

ויזואליזציה 2
מודל WWH – הסבר על הוויזואליזציה
<table dir="rtl"> <thead> <tr> <th>רכיב</th> <th>תוכן</th> </tr> </thead> <tbody> <tr> <td><strong>What – מה מוצג?</strong></td> <td> הגרף מציג את התפלגות גובה העסקאות (Deal Size Distribution) בקרב עשרת הסוכנים המובילים בחברה. לכל סוכן מוצגת עקומת צפיפות (Density Plot) הממחישה את השכיחות של סכומי העסקה השונים. בנוסף, הגרף מציג את החציון האישי של כל סוכן (קו לבן מרוסק), את החציון הגלובלי של כלל הסוכנים (קו אפור אנכי) ואת מספר העסקאות הכולל (N) לכל סוכן, כאשר הסוכנים מסודרים מלמעלה למטה לפי גובה החציון. </td> </tr> <tr> <td><strong>Why – למה בחרנו בגרף הזה?</strong></td> <td> מטרת הגרף היא לחשוף את "אישיות המכירה" של הסוכנים ולא רק את השורה התחתונה. הוא מאפשר להבדיל בין סוכנים שמבססים את ההכנסה שלהם על מעט עסקאות ענק ("ציידים") לבין סוכנים שעובדים בנפח גבוה של עסקאות קטנות ("חקלאים"). הבחנה זו קריטית להקצאה נכונה של סוכנים לאזורים או לקוחות מתאימים. </td> </tr> <tr> <td><strong>How – איך הגרף מציג את הנתונים?</strong></td> <td> הגרף הוא מסוג <strong>Ridge Plot</strong> (או Joyplot). ציר ה-X מייצג את שווי העסקה בשקלים (עד האחוזון ה-96 לנטרול חריגים קיצוניים), והציר האנכי מפוצל לשורות נפרדות לכל סוכן. השימוש בשטחים חופפים למחצה מאפשר השוואה קלה של צורת ההתפלגות. הקו המנחה האנכי (Global Med) משמש כנקודת ייחוס (Benchmark) שחותכת את כל הגרפים ומאפשרת לראות במבט אחד מי נמצא מעל ומתחת לנורמה הארגונית. </td> </tr> </tbody> </table>

<details> <summary><strong>לחץ להצגת הקוד המלא (Python)</strong></summary>

Python

import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd
import numpy as np
from matplotlib.ticker import FuncFormatter
from scipy.stats import gaussian_kde

# ==========================================
# STEP 1: Data Preparation
# ==========================================

# Rename columns for convenience
df.rename(columns={'סכום נטו הזמנה ': 'NetAmount', 'ערוץ ': 'Channel', 'מספר סוכן ': 'AgentID'}, inplace=True)

# Filter out noise (>50), keeping top outliers for accurate stats calculation
orders = df[df['NetAmount'] > 50].copy()
orders['AgentID_Str'] = "Agent " + orders['AgentID'].astype(str)

# Agent Selection: Select Top 10 agents by Total Revenue
top_agents_list = orders.groupby('AgentID_Str')['NetAmount'].sum().sort_values(ascending=False).head(10).index
data_agent = orders[orders['AgentID_Str'].isin(top_agents_list)].copy()

# Sort agents by Median deal size (Descending)
median_order = data_agent.groupby('AgentID_Str')['NetAmount'].median().sort_values(ascending=False).index

# Global Benchmarks
global_median = data_agent['NetAmount'].median()

# Set visual limit for X-axis (Zoom to 96% to hide extreme outliers in the plot)
viz_xlim = data_agent['NetAmount'].quantile(0.96)

# ==========================================
# STEP 2: Visualization Logic (Ridge Plot)
# ==========================================

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

# Initialize Grid
g = sns.FacetGrid(data_agent, row='AgentID_Str', hue='AgentID_Str',
                  aspect=10, height=1.3, row_order=median_order)

g.map(draw_comprehensive_density, 'NetAmount', color=joy_color)

# ==========================================
# STEP 3: Styling & Annotations
# ==========================================

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

print("Generating Ridge Plot...")
plt.show()
</details>

📊 Visualization Output (Screenshot)
<div align="center"> <img src="https://github.com/orelgrBGU/Diplomat_Visualization/blob/main/ridge_plot.png?raw=true" alt="Top 10 Agents Performance" width="80%" style="border: 1px solid #ccc; border-radius: 8px;"> </div>


הסבר על הגרף
הוויזואליזציה מאפשרת לנו לראות שלא כל ההכנסות נולדו שוות. הגרף חושף הבדל דרמטי באסטרטגיית המכירה בין הסוכנים המובילים: סוכנים כמו Agent 35 ו-Agent 25 (בראש הרשימה) מציגים "זנב" ארוך לימין והתפלגות שטוחה. הם מתפקדים כ"ציידים" – משיגים עסקאות בשווי גבוה מאוד (חציון סביב 40k₪) אך במספר עסקאות נמוך יחסית. לעומת זאת, הסוכנים בתחתית הרשימה (כמו Agent 42) מציגים "גבעה" צרה וגבוהה בצד השמאל. הם מתפקדים כ"חקלאים" – עובדים קשה על נפח עצום של עסקאות קטנות (כמעט 1,000 הזמנות בחציון של 9k₪ בלבד).

תובנה זו קריטית לניהול: היא מעידה שייתכן שאנו "מבזבזים" סוכנים חזקים על קווי חלוקה קמעונאיים קטנים, או להפך – שולחים סוכנים שמתמחים בנפח ללקוחות אסטרטגיים שדורשים מכירה מורכבת יותר. הגרף מציע לשקול התאמה מחדש של תיקי הלקוחות לפי פרופיל הסוכן.
