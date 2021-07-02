# Interative Visualization of Mobile Device Market Leaders
Finding mobile device market leaders through an interactive visualization and self-organizing mapping(SOM)

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























