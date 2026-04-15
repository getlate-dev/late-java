

# ListConversionDestinations200ResponseDestinationsInner


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | Destination identifier. Meta: pixel ID. Google: conversion action resource name.  |  [optional] |
|**name** | **String** |  |  [optional] |
|**type** | **String** | Present when the platform locks event type to the destination (Google conversion actions).  |  [optional] |
|**status** | [**StatusEnum**](#StatusEnum) |  |  [optional] |



## Enum: StatusEnum

| Name | Value |
|---- | -----|
| ACTIVE | &quot;active&quot; |
| INACTIVE | &quot;inactive&quot; |



