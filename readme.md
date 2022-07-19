# Experiment tracking for XGBoost projects

Ensure that you have the latest version of the Layer SDK: 

`pip install -U layer`


Layer allows you to keep track of your model artifacts,datasets and model versions.

Here is an example of how you can use Layer to log model metrics, parameters, evaluation metrics and charts in an XGBoost project.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1avRqBqA4rbutJwp78xHPMNyL4KiqZR2v?usp=sharing) 

## How to use the model 

```
import layer
my_model = layer.get_model("layer/xgboost/models/xgboost").get_train()
predictions = my_model.predict(np.array([[68,1,2,180,274,1,0,150,1,1.6,1,0,3]]))
predictions
#  ⠋  xgboost              ━━━━━━━━━━ LOADED [0:00:00] 
# array([0])
```

https://app.layer.ai/layer/xgboost/models/xgboost?w=1.5&w=1.4&w=1.3&w=1.2&w=1.1#Sample-predictions https://app.layer.ai/layer/xgboost/models/xgboost?w=1.5&w=1.4&w=1.3&w=1.2&w=1.1#Confusion-metrics https://app.layer.ai/layer/xgboost/models/xgboost?w=1.5&w=1.4&w=1.3&w=1.2&w=1.1#avg_precision https://app.layer.ai/layer/xgboost/models/xgboost