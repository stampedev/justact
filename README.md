# justact
Justact is the spritual successor of 
[particity](https://github.com/stampedev/particity)
, a project developed around 2015-2016 at Fraunhofer FOKUS, Dep. 
[Öffentliche IT](https://www.oeffentliche-it.de/)

Initially developed for Liferay CMS, this rewrite aims at providing
a more up to date implementation based upon spring(-boot).

## Status
Currently this project is in the early concept & design phase, 
so not much to see here (yet).

## Overview / temporary docs
At some point, documentation will be done using the
[arc42-method](https://arc42.org/)
, provided and maintained in the source at
[arc42](arc42)

### Basic concepts and goals
Justact provides a service platform for posting and browsing want-ads.
As such it comes with a prototype UI based upon angular to visualize the
basic concepts and workflows.

Justact is developed by keeping its focus on social engagement, as such
aiming to be easily deployed and maintained.

### Stakeholders and actors
... and their needs

Developers
- easy to participate in ongoing development
- easy to understand due to clear structure and documentation

Social engagement associations/societies
- easy setup & maintaining (config, updates, etc)
- web-based and mobile-friendly UI/UX to attract users

### Features and use-cases
General:
- web-based platform setup
- map-based approach on finding offers/want-ads (using filters, proximity search, etc)
- state-of-the-art authentication (i.e. OpenID/OAuth, U/P, 2FA/TOTP)
- rights/roles management for admins, organisations/editors, user/subscriber
- initial support for DE,EN - allow easy update for additional languages

Operator:
- hosts the platform / services
- adds / moderates new organisations
- provide basic domain-setup (i.e. topics & templates for posts)
- can manage all users (e.g. block / ban)

Organisations:
- self-registration that is moderated by platform operator
- maintain an organisation profile with contact and logo
- manage roles/rights for editors/contacts inside organisation
- editors can post want-ads on behalf of the organisation
- can invite users to join their organisation (i.e. as editors)

Posts:
- are moderated by organisation and/or platform operator
- contain details on the offer/advertisement, 
start/end publishing-date and geolocation
- are assigned to one or more topics

Users:
- minimal self-services (e.g. password, subscriptions, download personal data)
- can subscribe to topics or organisations and receive notifications (i.e. e-mail)
- can report organisations/offers to the operator

Long term:
- provide support for federation of platforms
- prototype Android-App