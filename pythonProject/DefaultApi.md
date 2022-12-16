# activity.DefaultApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**admin_activities_activities_get**](DefaultApi.md#admin_activities_activities_get) | **GET** /admin/activities/{activities} | 管理所有活动
[**admin_activity_acti_name_get**](DefaultApi.md#admin_activity_acti_name_get) | **GET** /admin/activity/{acti_name} | 管理活动信息
[**admin_review_post**](DefaultApi.md#admin_review_post) | **POST** /admin/review | 审核活动


# **admin_activities_activities_get**
> InlineResponse2006 admin_activities_activities_get(activities)

管理所有活动

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.DefaultApi(api_client)
    activities = 'activities_example' # str | 

    try:
        # 管理所有活动
        api_response = api_instance.admin_activities_activities_get(activities)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling DefaultApi->admin_activities_activities_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activities** | **str**|  | 

### Return type

[**InlineResponse2006**](InlineResponse2006.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **admin_activity_acti_name_get**
> InlineResponse20010 admin_activity_acti_name_get(acti_name)

管理活动信息

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.DefaultApi(api_client)
    acti_name = 'acti_name_example' # str | 

    try:
        # 管理活动信息
        api_response = api_instance.admin_activity_acti_name_get(acti_name)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling DefaultApi->admin_activity_acti_name_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **acti_name** | **str**|  | 

### Return type

[**InlineResponse20010**](InlineResponse20010.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |
**404** | 记录不存在 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **admin_review_post**
> InlineResponse2009 admin_review_post(activities=activities)

审核活动

### Example

```python
from __future__ import print_function
import time
import activity
from activity.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = activity.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with activity.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = activity.DefaultApi(api_client)
    activities = 'activities_example' # str |  (optional)

    try:
        # 审核活动
        api_response = api_instance.admin_review_post(activities=activities)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling DefaultApi->admin_review_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activities** | **str**|  | [optional] 

### Return type

[**InlineResponse2009**](InlineResponse2009.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 通过 |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

