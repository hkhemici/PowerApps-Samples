# Query the working hours of a user

This sample shows how to retrieve the working hours of a user by using the [QueryScheduleRequest](https://docs.microsoft.com/en-us/dotnet/api/microsoft.crm.sdk.messages.queryschedulerequest?view=dynamics-general-ce-9) message.

## How to run this sample

See [How to run samples](https://github.com/microsoft/PowerApps-Samples/blob/master/cds/README.md) for information about how to run this sample.

## What this sample does

The `QueryScheduleRequest` message is intended to be used in a scenario where it contains data that is needed to search the specified resource for an available time block that matches specified parameters.

## How this sample works

In order to simulate the scenario described in [What this sample does](#what-this-sample-does), the sample will do the following:

### Setup

1. Checks for the current version of the org.

### Demonstrate

1. The `WhoAMIRequest` message gets the current user's information.
2. The `QueryScheduleRequest` message retrieves the working hours of the current user.

### Clean up

1. Display an option to delete the sample data created in [Setup](#setup).
    The deletion is optional in case you want to examine the entities and data created by the sample. You can manually delete the records to achieve the same result.
