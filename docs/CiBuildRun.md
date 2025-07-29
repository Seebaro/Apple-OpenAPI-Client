# CiBuildRun


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**CiBuildRunAttributes**](CiBuildRunAttributes.md) |  | [optional] 
**relationships** | [**CiBuildRunRelationships**](CiBuildRunRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.ci_build_run import CiBuildRun

# TODO update the JSON string below
json = "{}"
# create an instance of CiBuildRun from a JSON string
ci_build_run_instance = CiBuildRun.from_json(json)
# print the JSON string representation of the object
print(CiBuildRun.to_json())

# convert the object into a dict
ci_build_run_dict = ci_build_run_instance.to_dict()
# create an instance of CiBuildRun from a dict
ci_build_run_from_dict = CiBuildRun.from_dict(ci_build_run_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


