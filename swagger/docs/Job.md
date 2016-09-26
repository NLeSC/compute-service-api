# ComputeServiceApi.Job

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** |  | 
**workflow** | **String** |  | 
**input** | [**CwlBinding**](CwlBinding.md) |  | 
**state** | **String** |  | 
**output** | [**CwlBinding**](CwlBinding.md) |  | 
**log** | **String** |  | 


<a name="StateEnum"></a>
## Enum: StateEnum


* `Waiting` (value: `"Waiting"`)

* `Running` (value: `"Running"`)

* `Success` (value: `"Success"`)

* `Canceled` (value: `"Canceled"`)

* `TemporaryFailure` (value: `"TemporaryFailure"`)

* `Failed` (value: `"Failed"`)

* `SystemError` (value: `"SystemError"`)




