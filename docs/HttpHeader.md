# HttpHeader


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**value** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.http_header import HttpHeader

# TODO update the JSON string below
json = "{}"
# create an instance of HttpHeader from a JSON string
http_header_instance = HttpHeader.from_json(json)
# print the JSON string representation of the object
print(HttpHeader.to_json())

# convert the object into a dict
http_header_dict = http_header_instance.to_dict()
# create an instance of HttpHeader from a dict
http_header_from_dict = HttpHeader.from_dict(http_header_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


