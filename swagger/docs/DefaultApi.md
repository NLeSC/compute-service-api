# ComputeServiceApi.DefaultApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**jobsGet**](DefaultApi.md#jobsGet) | **GET** /jobs | list of jobs
[**jobsJobIdCancelPost**](DefaultApi.md#jobsJobIdCancelPost) | **POST** /jobs/{jobId}/cancel | 
[**jobsJobIdDelete**](DefaultApi.md#jobsJobIdDelete) | **DELETE** /jobs/{jobId} | 
[**jobsJobIdGet**](DefaultApi.md#jobsJobIdGet) | **GET** /jobs/{jobId} | 
[**jobsPost**](DefaultApi.md#jobsPost) | **POST** /jobs | submit a new job
[**rootGet**](DefaultApi.md#rootGet) | **GET** / | Check if the server is working at all, returns some status info.


<a name="jobsGet"></a>
# **jobsGet**
> [Job] jobsGet()

list of jobs

get a list of all jobs, running, cancelled, or otherwise.

### Example
```javascript
var ComputeServiceApi = require('compute_service_api');

var apiInstance = new ComputeServiceApi.DefaultApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.jobsGet(callback);
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**[Job]**](Job.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="jobsJobIdCancelPost"></a>
# **jobsJobIdCancelPost**
> jobsJobIdCancelPost(jobId)



### Example
```javascript
var ComputeServiceApi = require('compute_service_api');

var apiInstance = new ComputeServiceApi.DefaultApi();

var jobId = "jobId_example"; // String | Job ID


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.jobsJobIdCancelPost(jobId, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **jobId** | **String**| Job ID | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="jobsJobIdDelete"></a>
# **jobsJobIdDelete**
> jobsJobIdDelete(jobId)



### Example
```javascript
var ComputeServiceApi = require('compute_service_api');

var apiInstance = new ComputeServiceApi.DefaultApi();

var jobId = "jobId_example"; // String | Job ID


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.jobsJobIdDelete(jobId, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **jobId** | **String**| Job ID | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="jobsJobIdGet"></a>
# **jobsJobIdGet**
> Job jobsJobIdGet(jobId)



### Example
```javascript
var ComputeServiceApi = require('compute_service_api');

var apiInstance = new ComputeServiceApi.DefaultApi();

var jobId = "jobId_example"; // String | Job ID


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.jobsJobIdGet(jobId, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **jobId** | **String**| Job ID | 

### Return type

[**Job**](Job.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a name="jobsPost"></a>
# **jobsPost**
> jobsPost(workflow, opts)

submit a new job

submit a new job from a workflow definition

### Example
```javascript
var ComputeServiceApi = require('compute_service_api');

var apiInstance = new ComputeServiceApi.DefaultApi();

var workflow = "workflow_example"; // String | location of cwl workflow definition.

var opts = { 
  'body': new ComputeServiceApi.CwlBinding() // CwlBinding | input binding for cwl workflow (json key value pairs)
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.jobsPost(workflow, opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workflow** | **String**| location of cwl workflow definition. | 
 **body** | [**CwlBinding**](CwlBinding.md)| input binding for cwl workflow (json key value pairs) | [optional] 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a name="rootGet"></a>
# **rootGet**
> rootGet()

Check if the server is working at all, returns some status info.

### Example
```javascript
var ComputeServiceApi = require('compute_service_api');

var apiInstance = new ComputeServiceApi.DefaultApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.rootGet(callback);
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

