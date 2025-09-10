# Event Types Schema - `event-type-schema.json`

This schema defines the known event types that are used in the Event Notification API.

This list is maintained alongside the Event Notification API which will also define the mandatory events that must be
supported by all API Providers. Any changes to the list of mandatory events will require a new version of the standards
to be published. This list also includes the names of optional events that have been agreed by the API Centre working
groups. These optional event types can be updated outside of publishing a new standards version.

API Providers can also define their own custom event types, these would be namespaced to the API provider to avoid
collisions with the standard event types.

This has been split out so that instead of API Providers creating custom event types with different names and the same
meaning. They can propose a new Optional event type be added to the standard list for all API Providers to use. 

| Event Type                                                               | Mandatory/Optional | Description                                                                                                              |
|--------------------------------------------------------------------------|--------------------|--------------------------------------------------------------------------------------------------------------------------|
| `urn:nz:co:paymentsnz:apicentre:events:account-access-consent-revoked`   | Mandatory          | Inform the data requestor when an account access consent created by them is revoked by the customer at the data holder   |
| `urn:nz:co:paymentsnz:apicentre:events:enduring-payment-consent-revoked` | Mandatory          | Inform the data requestor when an enduring payment consent created by them is revoked by the customer at the data holder |
| `urn:nz:co:paymentsnz:apicentre:events:xyz`                              | Optional           | Example optional event type to show how they would appear in the schema. (will remove this line in future)               |