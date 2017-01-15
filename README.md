# Stargazer

A wallet application for the [Stellar](https://stellar.org) platform. Desktop and Mobile.


## Main features:

* Multiple accounts

* Multiple assets
	* Issue/Redeem
	* Send/Receive/Trade

* Multiple networks

* Import/export accounts
	* QR code
	* Manual input

* Create/receive payment requests

* Add contacts
	* using QR code
	* from a transaction

* Add comments to transactions

* Federated addresses


## Security

All private keys are stored in localStorage, encrypted or not. Within the app, key decryption and transaction signing all take place inside the `Keychain` service in `app/core/services/keychain.js`. The only time an unencrypted private key leaves that service is when an account is being exported and you're not using password protection.


## Translations

- Go to [https://crowdin.com/project/stargazer]() and sign up.
- Select the language you want to translate.
- Select the "en.json" file.
- Start translating words/phrases.

*NB: Some of the phrases contains placeholders, e.g. `{{key}}`, where the placeholder `key` mustn't be translated.
Some of the phrases, specifically the `XX days/hours/minutes/seconds ago` ones, have both a singular and a plurar form that should be translated.*


## License

**Stargazer** is released under the **GNU Affero General Public License v3** (AGPL), except for the following files:

* app/core/controllers/scanner.js
* app/core/directives/qr-scanner.js
* app/core/services/platform-info.js

which originate from **Copay**, and are made available under the terms of the **MIT License**.

Copyright &copy; 2016-2017 Future Tense, LLC
