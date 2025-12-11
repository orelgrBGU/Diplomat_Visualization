
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

   
      
      </td>
    </tr>
  </tbody>
</table>
##קוד pyton 
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


