# platform-services-wordpress

[![Lifecycle:Experimental](https://img.shields.io/badge/Lifecycle-Experimental-339999)](https://github.com/bcgov/repomountie/blob/master/doc/lifecycle-badges.md)

This repository collects code snippets and configuration details for the [Cloud.gov.bc.ca multi-site WordPress instance](https://cloud.gov.bc.ca/). As this site network is provided as a hosted service, our code is placed into the site through the WordPress GUI at runtime.

## Contact Info

Please contact the Platform Services Team via [Rocket.Chat](https://developer.gov.bc.ca/Steps-to-join-Rocket.Chat) or by [email](mailto:PlatformServicesTeam@gov.bc.ca) with questions.

## Vendor Info

The code snippets included in this repository are used in a WordPress v6 multi-site instance provided by the [GDX Digital Engagement Solutions team](https://dir.gov.bc.ca/gtds.cgi?show=Branch&organizationCode=CITZ&organizationalUnitCode=GDX%2dDES) using their "Bcgov Engagement" theme.

## Repo Overview

- `./src/<site>/additional-css.css`

  - CSS styles that get applied to a particular site through the Additional CSS menu (from WP admin panel, Appearance -> Customize -> Additional CSS).

- `./src/alert-banner.html`
  - HTML markup plus a `<style>` block to create an instance of the `warning` style [alert banner from the Design System](https://developer.gov.bc.ca/Design-System/Alert-Banners). This was developed for use on the Private Cloud site's homepage, but user testing revealed that users found this confusing. This code isn't used on any of our sites at this time.
