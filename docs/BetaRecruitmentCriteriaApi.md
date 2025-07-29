# openapi_client.BetaRecruitmentCriteriaApi

All URIs are relative to *https://api.appstoreconnect.apple.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**beta_recruitment_criteria_create_instance**](BetaRecruitmentCriteriaApi.md#beta_recruitment_criteria_create_instance) | **POST** /v1/betaRecruitmentCriteria | 
[**beta_recruitment_criteria_delete_instance**](BetaRecruitmentCriteriaApi.md#beta_recruitment_criteria_delete_instance) | **DELETE** /v1/betaRecruitmentCriteria/{id} | 
[**beta_recruitment_criteria_update_instance**](BetaRecruitmentCriteriaApi.md#beta_recruitment_criteria_update_instance) | **PATCH** /v1/betaRecruitmentCriteria/{id} | 


# **beta_recruitment_criteria_create_instance**
> BetaRecruitmentCriterionResponse beta_recruitment_criteria_create_instance(beta_recruitment_criterion_create_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_recruitment_criterion_create_request import BetaRecruitmentCriterionCreateRequest
from openapi_client.models.beta_recruitment_criterion_response import BetaRecruitmentCriterionResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.BetaRecruitmentCriteriaApi(api_client)
    beta_recruitment_criterion_create_request = openapi_client.BetaRecruitmentCriterionCreateRequest() # BetaRecruitmentCriterionCreateRequest | BetaRecruitmentCriterion representation

    try:
        api_response = api_instance.beta_recruitment_criteria_create_instance(beta_recruitment_criterion_create_request)
        print("The response of BetaRecruitmentCriteriaApi->beta_recruitment_criteria_create_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BetaRecruitmentCriteriaApi->beta_recruitment_criteria_create_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **beta_recruitment_criterion_create_request** | [**BetaRecruitmentCriterionCreateRequest**](BetaRecruitmentCriterionCreateRequest.md)| BetaRecruitmentCriterion representation | 

### Return type

[**BetaRecruitmentCriterionResponse**](BetaRecruitmentCriterionResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**201** | Single BetaRecruitmentCriterion |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **beta_recruitment_criteria_delete_instance**
> beta_recruitment_criteria_delete_instance(id)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.BetaRecruitmentCriteriaApi(api_client)
    id = 'id_example' # str | the id of the requested resource

    try:
        api_instance.beta_recruitment_criteria_delete_instance(id)
    except Exception as e:
        print("Exception when calling BetaRecruitmentCriteriaApi->beta_recruitment_criteria_delete_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 

### Return type

void (empty response body)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**409** | Request entity error(s) |  -  |
**204** | Success (no content) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **beta_recruitment_criteria_update_instance**
> BetaRecruitmentCriterionResponse beta_recruitment_criteria_update_instance(id, beta_recruitment_criterion_update_request)

### Example

* Bearer (JWT) Authentication (itc-bearer-token):

```python
import openapi_client
from openapi_client.models.beta_recruitment_criterion_response import BetaRecruitmentCriterionResponse
from openapi_client.models.beta_recruitment_criterion_update_request import BetaRecruitmentCriterionUpdateRequest
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.appstoreconnect.apple.com
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://api.appstoreconnect.apple.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): itc-bearer-token
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.BetaRecruitmentCriteriaApi(api_client)
    id = 'id_example' # str | the id of the requested resource
    beta_recruitment_criterion_update_request = openapi_client.BetaRecruitmentCriterionUpdateRequest() # BetaRecruitmentCriterionUpdateRequest | BetaRecruitmentCriterion representation

    try:
        api_response = api_instance.beta_recruitment_criteria_update_instance(id, beta_recruitment_criterion_update_request)
        print("The response of BetaRecruitmentCriteriaApi->beta_recruitment_criteria_update_instance:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BetaRecruitmentCriteriaApi->beta_recruitment_criteria_update_instance: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| the id of the requested resource | 
 **beta_recruitment_criterion_update_request** | [**BetaRecruitmentCriterionUpdateRequest**](BetaRecruitmentCriterionUpdateRequest.md)| BetaRecruitmentCriterion representation | 

### Return type

[**BetaRecruitmentCriterionResponse**](BetaRecruitmentCriterionResponse.md)

### Authorization

[itc-bearer-token](../README.md#itc-bearer-token)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Parameter error(s) |  -  |
**401** | Unauthorized error(s) |  -  |
**403** | Forbidden error |  -  |
**404** | Not found error |  -  |
**422** | Unprocessable request entity error(s) |  -  |
**200** | Single BetaRecruitmentCriterion |  -  |
**409** | Request entity error(s) |  -  |
**429** | Rate limit exceeded error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

