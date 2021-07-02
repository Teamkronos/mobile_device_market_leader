# Topic: Finding Mobile Device Market Leaders Through An Interactive Visualization & Self-Organizing Mapping(SOM)

* The dataset contains 213 companies that produced different mobile devices from 1989 to 2012.
* There are 16 dimensions with 3162 rows
* The goal of this project is to extract meaningful information from a dataset through a interactive visualization method and SOM.
* Used Python libraries - Plotly and Dash to extract valuable information for this project.
* Used SOM and dashboard as tools in creating different visualisations to investigate which devices or companies are the most successful in leading the market.

### Exploratary Data Analysis
The main spreadsheet in our data set primarily includes mobile device names (nominal), release date and year (ordinal) and 12 ratio type attributes which can be split into two categories:

• Performance Based Attributes - RAM, CPU, Storage, Pixel Density; A larger values is more desirable to consumers

• Dimensional Attributes - Screen Width, Length and Diagonal, Display Diagonal, Length and Width, Volume and Mass; A larger value is not necessarily more desirable to consumers

Scatter Plot: To find trends or seasonality over time, we provide scatter plots of the feature data with respect to time. Some interesting pattern can be seen in the following scatter plot (Figure 3): RAM Capacity, Storage, CPU Clock and Pixel Density. These plots show horizontal periodic trend lay up along the y-axis. Such period can be explained by innovation diffusion theory and each period corresponds to an innovation diffusion period

![](https://github.com/Teamkronos/mobile_device_market_leader/blob/main/images/diffusion.PNG)
![](https://github.com/Teamkronos/mobile_device_market_leader/blob/main/images/1_scatterplot.PNG)

Density Plot with Respect to the Features:  Positively skewed distribution can be observed on width,length, depth, volume and mass features on Figure 4 . This is due to devices such as tablets, which have significantly longer, wider and thicker measurement compared to an average mobile phone device. A density plot of these five features reveals a normal distribution, and the median of these attributes represents the most popular dimensions that customers have for mobile devices.

![](https://github.com/Teamkronos/mobile_device_market_leader/blob/main/images/3_densityplot.PNG)

### Interactive Dashboard
![](https://github.com/Teamkronos/mobile_device_market_leader/blob/main/images/0_mainview.PNG)

![](https://github.com/Teamkronos/mobile_device_market_leader/blob/main/images/4_diffusionperiod.PNG)

### KGI AND KPIs
Our Key Goal Indicator (KGI) is how successful companies and mobile devices are at leading the market. To measure this KGI, we provide three Key Performance Indicators (KPI), two of which are based on hardware attributes (Beating the Trend and Earliest Adapters). Meanwhile Closest to Median is based on dimensional attributes.

1) Beating the Trend: A linear fit is calculated for the selected attribute which is displayed in the scatter plot and each mobile device is given a score based on the residuals of the linear fit, then color coded accordingly. The companies are scored by the sum of all their device’s scores. An additional attribute named sum of attributes is provided, which is a normalized score of the sum of all performance based attributes, which is used for identifying how mobile devices compare with respect to all performance attributes. The market leading device is represented by the scatter point having the most dark red color, and the hove label can be used to identify the name and exact score of that particular device.

2) Earliest Adapters: When plotting the performance based attributes, it is frequently seen that mobile devices are clustered around discrete steps. This happens because mobile device manufacturers often follow standards such as RAM capacity doubling at each new generation, or manufacturers using the same hardware components. Each discrete step can be considered as a new market, and the first device in each step is considered to be the market leader

3) Closest to Median: For most of the attributes corresponding to the size and dimensions of the mobile device, a larger attribute value is not necessarily better. For these attributes we provide the closest to median KPI. We decided that median should be selected over mean to overcome any outlier influences. We decided to include Display Diagonal, Display Width and Display Length in this method rather than Earliest Adopter Method even though these features show a clear trend in their respective time series plots. For dimensional attributes such as size and shape of the mobile device, we can not assume that a larger value is necessarily better compared to a smaller one, and the identification of an optimal value can be very subjective. Nonetheless, we considered the median of each attribute to be the optimal value for each attribute, and we scored mobile devices based on their proximity to the median.

### Results
![](https://github.com/Teamkronos/mobile_device_market_leader/blob/main/images/5_result1.PNG)
![](https://github.com/Teamkronos/mobile_device_market_leader/blob/main/images/6_result2.PNG)
![](https://github.com/Teamkronos/mobile_device_market_leader/blob/main/images/7_result3.PNG)














































