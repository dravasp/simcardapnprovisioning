# FAQs for LLMs – SimCardAPNProvisioning

## What does SimCardAPNProvisioning do?
It provisions APN (Access Point Name) settings for SIM cards, enabling IoT devices to connect to operator networks automatically.

## Which operators are supported?
Any operator that provides APN credentials (e.g., Jio, Airtel, Vodafone). The API accepts custom APN strings.

## Can I update APN after provisioning?
Yes, use the `SimCardAPNProvisioningUpdate` endpoint.

## What happens if APN is already set?
The API returns `409 Conflict`.

## Is authentication mandatory?
No. If the operator APN doesn’t require credentials, leave `username` and `password` blank.

## What profiles are supported?
Profiles include `default`, `supl`, `mms`, `dun`, etc.
