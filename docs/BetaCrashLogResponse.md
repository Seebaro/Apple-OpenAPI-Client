# BetaCrashLogResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**BetaCrashLog**](BetaCrashLog.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.beta_crash_log_response import BetaCrashLogResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BetaCrashLogResponse from a JSON string
beta_crash_log_response_instance = BetaCrashLogResponse.from_json(json)
# print the JSON string representation of the object
print(BetaCrashLogResponse.to_json())

# convert the object into a dict
beta_crash_log_response_dict = beta_crash_log_response_instance.to_dict()
# create an instance of BetaCrashLogResponse from a dict
beta_crash_log_response_from_dict = BetaCrashLogResponse.from_dict(beta_crash_log_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


