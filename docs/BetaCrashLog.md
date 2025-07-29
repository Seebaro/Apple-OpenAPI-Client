# BetaCrashLog


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**BetaCrashLogAttributes**](BetaCrashLogAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.beta_crash_log import BetaCrashLog

# TODO update the JSON string below
json = "{}"
# create an instance of BetaCrashLog from a JSON string
beta_crash_log_instance = BetaCrashLog.from_json(json)
# print the JSON string representation of the object
print(BetaCrashLog.to_json())

# convert the object into a dict
beta_crash_log_dict = beta_crash_log_instance.to_dict()
# create an instance of BetaCrashLog from a dict
beta_crash_log_from_dict = BetaCrashLog.from_dict(beta_crash_log_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


