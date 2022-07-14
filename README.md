
# {app-name} App

Experiment to extend Ontario's [Verify Ontario](https://github.com/ongov/OpenVerify) app to verify formats other than "SMART Health Card".

## Overview

This is a React Native app designed work on Android and iOS devices.

{app-name} gives businesses and organizations a quick, easy, and trusted way to scan and confirm that visitors are fully vaccinated.

The app scans the QR code on vaccine certificates.

After scanning a QR code the app will display: a green checkmark indicating that it meets vaccine requirements, a red X for an invalid certificate, or a yellow warning indicating that the QR code cannot be read.

Open Verify verifies most government issued SMART® Health Card  QR codes including:
- Alberta
- British Columbia
- Manitoba
- New Brunswick
- Newfoundland & Labrador
- Northwest Territories
- Nova Scotia
- Nunavut
- Prince Edward Island
- Quebec
- Saskatchewan
- Yukon
- Canadian Armed Forces
- Global Affairs Canada

- Cayman Islands Health Services Authority
- Connecticut Department of Public Health
- Delaware Immunization Program
- Government of Puerto Rico
- Illinois Department of Public Health
- State of California
- State of Colorado
- State of Hawaii
- State of Louisiana
- State of New Jersey
- State of New York
- State of Utah
- Sydney Local Health District
- Virginia Department of Health
- Washington State Department of Health

## Local setup

#### 1. Clone the repository

```bash
git clone https://github.com/ahebbdel/OpenVerify
```

#### 2. Install dependencies

```bash
cd OpenVerify
yarn install
```

#### 3. Install pods

```bash
yarn run update:pods
```

#### 4. Environment config

```bash
cp .env.template .env
```

API_URL env variable points to the URL hosting the rules, public keys and minimum mandatory app version. Adjust the value accordingly.

#### 5. Launch app (development mode)

##### iOS

```bash
yarn run ios
```

#TODO: @amos add steps about getting xcode, developer.apple account, whatever else I need to do to get this running.

##### Android

```bash
yarn run android
```

## Rules, Public keys and Minimum mandatory app version

These are ONTARIO's public access endpoints for:

[Rules](https://files.ontario.ca/apps/verify/verifyRulesetON.json)

[Public keys](https://files.ontario.ca/apps/verify/verifyRulesetON.json)

[Minimum mandatory app version](https://files.ontario.ca/apps/verify/minimumVersion.json)

>amos -  Ontario's app has 3 links, but 2 are verifyRulesetOn.json, I've tried copying them to gh. 

#TODO: @amos paste links to github rawcontent of those two uploaded files, change path in .env to point to them.

## Vulnerability disclosure policy

#TODO: write unhackable code.