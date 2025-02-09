# Clean up history for a queue (early bound)

 This sample shows how to clean up the history for the queue by using [RemoveFromQueueRequest](https://docs.microsoft.com/en-us/dotnet/api/microsoft.crm.sdk.messages.removefromqueuerequest?view=dynamics-general-ce-9) with inactive items. It finds completed phone calls in the queue and removes the associated queue items.

## How to run this sample

See [How to run samples](https://github.com/microsoft/PowerApps-Samples/blob/master/cds/README.md) for information about how to run this sample.

## What this sample does

The `RemoveFromQueueRequest` message is intended to be used in a scenario to clean up the queue history with inactive items.

## How this sample works

In order to simulate the scenario described in [What this sample does](#what-this-sample-does), the sample will do the following:

### Setup

1. Creates a queue instance and set its property values.
2. Creates a phone call activity instance and also queueitems instance and initializes its properties.
3. Marks the phone call as completed.

### Demonstrate

1. Retrieves the queueitem with inactive phone calls from a queue using the [RemoveFromQueueRequest](https://docs.microsoft.com/en-us/dotnet/api/microsoft.crm.sdk.messages.removefromqueuerequest?view=dynamics-general-ce-9) message.

### Clean up

1. Display an option to delete the records created in [Setup](#setup).

    The deletion is optional in case you want to examine the entities and data created by the sample. You can manually delete the records to achieve the same result.
