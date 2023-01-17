# Employee Burnout Rate Prediction
## Predict if your employee will Burn Out
Understanding what will be the Burn Rate for the employee working in an organization based on the current pandemic situation where work from home is a boon and a bane. How are employees' Burn Rate affected based on various conditions provided?
當前在家工作大流行的情況下，欲了解在組織中工作員工的工作疲勞率是多少。根據提供的各種條件，以AI與機器學習的現有module來推估員工的疲勞率如何受到影響

## Dataset Description
- Employee ID: The unique ID allocated for each employee
- Date of Joining: The date-time when the employee has joined the organization (example: 2008-12-30)
- Gender: The gender of the employee (Male/Female)
- Company Type: The type of company where the employee is working (Service/Product)
- WFH Setup Available: Is the work from home facility available for the employee (Yes/No)
- Designation: The designation of the employee of work in the organization.(In the range of [0.0, 5.0] where bigger is higher designation.)
- Resource Allocation: The amount of resource allocated to the employee to work, ie. number of working hours.(In the range of [1.0, 10.0] where higher means more resource)
- Mental Fatigue Score: The level of fatigue mentally the employee is facing.(In the range of [0.0, 10.0] where 0.0 means no fatigue and 10.0 means completely fatigue)
- Burn Rate: The value we need to predict for each employee telling the rate of Bur out while working.(In the range of [0.0, 1.0] where the higher the value is more is the burn out)

## Algorithms
將數據進行資料前處理(特徵篩選、TargetEncoding)後，套入近期熱門之機器學習演算法建立多種模型，並使用 Optuna 預設之 TPESampler 進行超參數優化。
[XGBRegressor 程式檔]
[LGBMRegressor 程式檔]
[CatBoostRegressor 程式檔]
[EnsembleRegressor 程式檔]
[Tensorflow 框架建立之深度學習模型 程式檔]

