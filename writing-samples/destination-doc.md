# Destination Integration Doc

> This is a sanitised portfolio version of documentation work created in a production environment. Certain details and implementation specifics have been modified or omitted for confidentiality. For the live doc, [see Twilio Docs](https://twilio.com/docs/segment/connections/destinations/catalog/actions-SampleTool).

## Overview

Developer-facing integration documentation for connecting Twilio Segment event data to third-party analytics and reporting platforms.

This documentation focused on onboarding users to a destination integration while explaining supported methods, setup requirements, and expected event behaviour.

## Audience

- Developers
- Data and analytics teams
- Technical implementation users

## Skills demonstrated

- Developer documentation
- Integration onboarding
- API and event-spec documentation
- Technical reference writing
- Docs-as-code workflows
- MDX authoring

## Documentation considerations

This documentation needed to balance:
- onboarding clarity
- technical accuracy
- scannability
- consistency with other Segment destinations documentation

The structure prioritised:
- concise setup instructions
- reusable formatting patterns
- implementation-focused examples
- quick access to supported method behaviour

## Example excerpt

````md

[SampleTool] lets you sync YourTool events and identities data with SampleTool. SampleTool creates queryable tables that you can use to build custom reports and dashboards.

This destination is maintained by SampleTool. For any issues with the destination, [contact the SampleTool support team].

## Getting started

1. From your workspace's [destination catalog], search for "SampleTool".
2. Select "SampleTool" and click **Add destination**.
3. Select an existing Source to connect to SampleTool.
4. Go to the [SampleTool dashboard], find and copy the **Environment** slug and **API key**. 
5. Enter the **Environment** slug and **API key** in the SampleTool destination settings in your workspace.

## Supported methods

### Page
If you aren't familiar with the Spec, take a look at the [Page method documentation] to learn about what it does. An example call would look like:

```js
 
    service.page();
```

YourTool sends Page calls to SampleTool, which are stored as a `$pageview` event in the `platform_name.main.events` table.

### Track

If you aren't familiar with the Spec, take a look at the [Track method documentation] to learn about what it does. An example call would look like:

```js

    service.track("Login Button Clicked");
```
YourTool sends Track calls to SampleTool using the event name you provide, which are stored in the `platform_name.events` table.

## Additional information

- Data is synced in real time, so you can explore and analyze it immediately.
- SampleTool automatically structures incoming events and identities into resolved
and queryable analytical tables under the `SampleTool.analytics` schema.
````