# Data-Transformation
Transforming case.json file into three different .csv files using python pandas
In this project, we will convert case.json file into three csv files. The definition of three csv files are presented below:

### 1. CuratedOfferOptions.csv

CurationProvider: in quotes
OfferId: in quotes
DealerId: in quotes
UniqueOptionId: in quotes
OptionId: in quotes
IsMobileDealer: without quotes
IsOpen: without quotes
Eta: in quotes
ChamaScore: without quotes
ProductBrand: in quotes
IsWinner: without quotes
MinimumPrice: without quotes
MaximumPrice: without quotes
DynamicPrice: without quotes
FinalPrice: without quotes
DefeatPrimaryReason: in quotes
DefeatReasons: in quotes
EnqueuedTimeSP: DD/MM/YYYY (converted to Brasilian timezone - UTC-3)

### 2. DynamicPriceOptions.csv

Provider: in quotes
OfferId: in quotes
UniqueOptionId: in quotes
BestPrice: without quotes
EnqueuedTimeSP: DD/MM/YYYY (converted to Brasilian timezone - UTC-3)

### 3. DynamicPriceRange.csv

Provider: in quotes
OfferId: in quotes
MinGlobal: without quotes
MinRecommended: without quotes
MaxRecommended: without quotes
DifferenceMinRecommendMinTheory: without quotes
EnqueuedTimeSP: DD/MM/YYYY (converted to Brasilian timezone - UTC-3)  

### Data Description  

There is one file case.json. Below is an example of a single record from this file:

```python
{
    "EnqueuedTimeUtc": "2021-09-05 08:04:08 UTC",
    "EventName": "DynamicPrice_Result",
    "Payload": "{\"provider\":\"ApplyDynamicPriceRange\",\"offerId\":\"a6611d55-9624-4381-8cdd-323ee3689241\",\"algorithmOutput\":{\"min_global\":85.0,\"min_recommended\":87.2,\"max_recommended\":97.65,\"differenceMinRecommendMinTheory\":2.2}}"
}
```
