The Weather Sensory Data Prediction based on LSTM
=================================================
2011-13330 SNU CLS Seokmo-Yoo, August 2020.

Based on Long Short Term Memory(Sepp Hochreiter et al. 1997), which is effective model to predict time series data, I developed a simple prediction model of temperature and precipitation in weather sensory data. After training the model by observed data, I compared the result with the real data and analyzed the error of the result by numerical methods to discuss about accuracy.

## Methodology
Check out `snu2020-graduation-thesis.ipynb` for detail.
- using Tensorflow Keras in Python 3

## Model
<img src="figs/model.png">

- LSTM Layer(Unit: 100)
- Dense Layer(Unit: 1)

## Result
### Average Temperature
- Total test set
<img src="figs/avgtmp_whole.png">

- Lastest 120 days test set
<img src="figs/avgtmp_120days.png">

- Training loss by epochs
<img src="figs/avgtmp_loss.png">

- Scatter plot of ground truths verus predicted values
<img src="figs/avgtmp_scatter.png">

### Minimum Temperature
- Total test set
<img src="figs/mintmp_whole.png">

- Lastest 120 days test set
<img src="figs/mintmp_120days.png">

- Training loss by epochs
<img src="figs/mintmp_loss.png">

- Scatter plot of ground truths verus predicted values
<img src="figs/mintmp_scatter.png">

### Maximum Temperature
- Total test set
<img src="figs/maxtmp_whole.png">

- Lastest 120 days test set
<img src="figs/maxtmp_120days.png">

- Training loss by epochs
<img src="figs/maxtmp_loss.png">

- Scatter plot of ground truths verus predicted values
<img src="figs/maxtmp_scatter.png">

### Daily Precipitation
- Total test set
<img src="figs/preci_whole.png">

- Lastest 120 days test set
<img src="figs/preci_120days.png">

- Training loss by epochs
<img src="figs/preci_loss.png">

- Scatter plot of ground truths verus predicted values
<img src="figs/preci_scatter.png">
