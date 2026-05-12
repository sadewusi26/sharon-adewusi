# Short Code Senders 

> This is a sanitised portfolio version of documentation work created in a production environment. Certain details and implementation specifics have been modified or omitted for confidentiality. For the live doc, [see Twilio Docs](https://twilio.com/docs/numbers-and-senders/short-codes).

## Overview

Task-based documentation covering short code sender setup, registration, and compliance workflows within Twilio Console.

## Audience

- Developers
- Messaging customers
- Compliance and onboarding users

## Skills demonstrated

- Task-based documentation
- Docs-as-code workflows
- MDX authoring
- Regulatory/compliance guidance
- Product onboarding documentation
- Technical usability and scannability

## Example excerpt

``` md

<Warning title="Regional availability">
Short codes are only available in the United States, Canada, and the United Kingdom, and are subject to local regulations.
If you want to use short code numbers in a country that isn't supported, contact your [Account manager] to discuss options.
</Warning>

[Short codes] are three- to seven-digit numeric sender IDs designed for high-volume, two-way messaging over [SMS] and [MMS]. In the **Short Codes** tab of the **Senders** page, you can track and manage your short code registrations and active short codes.

## Setup and registration

Short codes require registration before they can be used. Regulatory requirements vary by country.
You can set up a short code either from **Senders** or from the [**Compliance Portal**]. To set up a short code from the **Compliance Portal**, click **Create Registration**, and follow the on-screen prompts to provide the required information.
To submit a short code compliance registration, follow the steps on how to [create a registration for short codes] in the Compliance Portal.

## Getting started

To set up a new short code from **Senders**:

1. Sign in to the [console] and go to **Products > Senders** in the side navigation.
2. Go to the **Short Codes** tab and click **Set up a new short code**.
3. Click **Request a Short code**.
4. Follow the on-screen prompts to provide the required information. During setup, you'll be guided through the registration steps for your selected country.

<Info title="Non-US Codes">

If you're setting up a non-US short code, select **Short codes (non-US)** in the side navigation and click **Request a Short code**. Select the country where you plan to use the short code.
</Info>

### Registration and the Compliance Portal

As part of the setup process, you're prompted to create a compliance profile in the Compliance Portal if you don't already have one. For more details, see [Compliance Profiles].

```