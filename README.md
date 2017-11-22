# Stripe Country Specs in JSON Format

Have you ever wanted to implement Stripe's 
[Required Verification Information](https://stripe.com/docs/connect/required-verification-information) guidelines for
Stripe Connect Custom? Sure, we've all been there at some point in our life.

This repository is a direct dump of the country spec for all supported countries, in JSON format.

Each folder in this repository represents a new update and is named by date.

Description of files:

1. default.json - A direct dump of all Country Spec objects in JSON format, untouched and pure.
2. default.min.json - Same as above, but minified.
3. with-country-label.json - Each Country Spec object now has a "label" attribute, which lists the country name.
4. with-country-label.min.json - Same as above, but minified.

Tip: These JSON files are large. If you intend on serving them client-side, consider removing as much data as possible
to lower the total download size.

## Prefer a CSV File Dump?

The above page lists out the requirements in a nice table, and offers a 
[CSV file](https://stripe.com/files/connect/Stripe_Connect_Custom_Identity_Verification.csv) as well.

## Prefer API Access?

The JSON dumps in this repository are grabbed directly from the Stripe API. You can do it too if you try hard enough:

[Country Specs API Docs](https://stripe.com/docs/api#country_specs)

## License

This repository is public domain, except for any license Stripe imposes on their data. Please refer to Stripe's terms if you
are concerned with licensing.