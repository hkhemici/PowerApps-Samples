# Promote an email message

This sample shows how to create an email activity instance from the specified email message in Dynamics 365 by using the [DeliverPromoteEmailRequest](https://docs.microsoft.com/en-us/dotnet/api/microsoft.crm.sdk.messages.deliverpromoteemailrequest?view=dynamics-general-ce-9) message.

## How to run this sample

See [How to run samples](https://github.com/microsoft/PowerApps-Samples/blob/master/cds/README.md) for information about how to run this sample.

## What this sample does

The `DeliverPromoteEmailRequest` message is intended to be used in a scenario where it contains data that is needed to create an email activity record from the specified email message.

## How this sample works

In order to simulate the scenario described in [What this sample does](#what-this-sample-does), the sample will do the following:

### Setup

1. Checks for the current version of the org.

### Demonstrate

1. Creates a contact to send an email to (To: field).
2. The `WhoAmIRequest` retrieves the system user to send the email (From: field).
3. The `DeliverPromoteEmailRequest` message creates the request and also executes it.
4. Verify the success by defining anonymous types that define possible values for email status.
5. Queries the delivered email, and verify the status code is `sent`.

### Clean up

1. Display an option to delete the records created in [Setup](#setup).

    The deletion is optional in case you want to examine the entities and data created by the sample. You can manually delete the records to achieve the same result.
