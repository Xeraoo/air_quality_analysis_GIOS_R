# Air Quality Data Analysis Using giosimport

## 1. Purpose

The purpose of this exercise is to familiarize students with the **giosimport** package, in order to analyze air quality data focusing on PM10 and PM2.5 concentrations. The data we use is raw, requiring us to understand its format and use tools for processing. We conducted a statistical analysis to identify trends and observe dependencies between the various data points. Additionally, we reviewed legal standards regarding Air Quality Assessment in Poland, including station norms and permissible pollutant levels for PM10 and PM2.5. Finally, we documented our work in a technical report using **RMarkdown**, summarizing the entire workflow in **R**.

## 2. R (Programming Language)

**R** is an interpreted programming language and environment for statistical computing. It is commonly used in the analysis of environmental and spatial data as well as data visualization. Similar to the S language developed at Bell Laboratories, **R** was created by Robert Gentleman and Ross Ihaka at the University of Auckland. It combines features of functional and object-oriented programming, making it well-suited for interactive data analysis.

*[Source](https://pl.wikipedia.org/wiki/R_(język_programowania))*

## 3. R Markdown

**R Markdown** is a file format designed for generating dynamic documents using R. The file is written in a specific syntax that allows easy text formatting and embedding of code chunks (code written in **R**). **R Markdown** is a convenient method for producing HTML, PDF, and MS Word documents.

*[Source](https://rmarkdown.rstudio.com/articles_intro.html)*

## 4. giosimport

The **giosimport** package is designed for downloading and importing data from the Air Quality Portal managed by GIOŚ. Although these datasets should have a uniform structure, they often contain inconsistencies that complicate simple solutions. The project code tends to become lengthy, with much focus on acquiring and converting data into a suitable form.

The functions within the package create a file-based database on your local disk, which can occupy up to 700 MB of space. You can download selected parts of the database, allowing year-by-year data acquisition. Since historical data is not updated, it only needs to be downloaded once. Ensure proper file organization to avoid redundant downloads.

*[Source 1](https://rpubs.com/rzeszut/giosimport)*
*[Source 2](https://github.com/mrzeszut)*

## 5. GIOŚ Air Quality Portal

The Environmental Protection Inspection (GIOŚ) is responsible for monitoring and controlling environmental regulations and assessing the state of the environment in Poland. The Inspection consists of the Chief Inspectorate of Environmental Protection (GIOŚ) and 16 regional environmental protection inspectorates. The Chief Inspector of Environmental Protection oversees its activities.

Air quality monitoring, as part of the State Environmental Monitoring (PMŚ), is conducted in accordance with the Act of July 10, 1991, on the Environmental Protection Inspection. The tasks include air pollution measurements and evaluations in specific zones, monitoring urban background for PAHs, assessing PM2.5 pollution for the national exposure reduction target, and monitoring heavy metals, mercury, and PM2.5 chemical composition.

The purpose of air quality monitoring, as per Article 23 of the Environmental Protection Inspection Act, is to provide information on substance levels in ambient air, along with analysis results and assessments of air quality standard compliance.

*[Source](https://powietrze.gios.gov.pl/pjp/content/about_us)*

### 5.1 Station Characteristics

We selected the air quality monitoring station located in **Kielce**, at **Targowa 3**. The station's national code is **SkKielTargow**, and the international code is **PL0704A**. The station has been active since **2018-07-01** and is situated at an altitude of **269 m above sea level**. It is an urban station responsible for monitoring air quality within the city, owned by the Chief Inspectorate of Environmental Protection. This provides a structured overview of the project's goals, background on the tools used (R, R Markdown, and giosimport), and additional information about the GIOŚ air quality data portal and the specific air quality monitoring station in Kielce.

## 6. Conclusions and Summary

This project provided valuable insights into air quality in Kielce, focusing on PM10 and PM2.5 particulate matter levels, which are crucial for assessing public health and environmental protection. The analysis of data from the GIOŚ database led to the following conclusions:

1. **Seasonality of pollution**: Significant differences in particulate matter levels were observed depending on the season. The highest pollution levels occurred during winter, which is associated with increased home heating and reduced air circulation in the city. In contrast, PM10 and PM2.5 levels were notably lower in the summer months.

2. **Impact of meteorological factors**: The analysis of meteorological data showed that atmospheric conditions, such as temperature, humidity, and wind speed, significantly affect particulate matter concentrations. For example, higher wind speeds generally contributed to lower pollution levels by dispersing the particulates.

3. **Random Forest Model Performance**: The Random Forest model used in the project demonstrated strong predictive capabilities for air pollution levels based on the provided meteorological data. This method was effective in capturing the complex relationships between various environmental factors and pollution levels.

4. **Recommendations for further study**: Future research could explore the integration of additional data sources, such as real-time traffic or industrial activity, to further refine the forecasting models. Additionally, extending the analysis to other regions could provide a more comprehensive understanding of air quality dynamics in Poland.

In summary, the project successfully demonstrated the correlation between meteorological conditions and air pollution levels in Kielce, and the Random Forest model proved to be a valuable tool for forecasting pollution trends.

## 7. Screenshots

![Gestosc_prawdopodobienstwa-1](https://github.com/user-attachments/assets/1f2eca8a-47df-4cbd-822d-6470246d8d05)

![Histogram-1](https://github.com/user-attachments/assets/fe562311-cc01-48eb-a9b6-65ba537639ca)

![Poglądowe_wykesey-1](https://github.com/user-attachments/assets/9d5a02cd-4969-481c-8e5d-bcf73853aea3)

![Wykres_rozrzutu-1](https://github.com/user-attachments/assets/d9421cab-c1b7-44a9-8af2-9b38dd505fb6)

![zroznicowanie-1](https://github.com/user-attachments/assets/a1b52283-d273-4467-8298-033fbee658ee)




