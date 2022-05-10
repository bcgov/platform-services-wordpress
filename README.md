# platform-services-wordpress

[![Lifecycle:Experimental](https://img.shields.io/badge/Lifecycle-Experimental-339999)](https://github.com/bcgov/repomountie/blob/master/doc/lifecycle-badges.md)

This repository collects code snippets and configuration details for the [Platform Services Cloud PaaS WordPress site](https://platform-services-dev.apps.silver.devops.gov.bc.ca/). Since this site is provided as a hosted service, our code is placed into the site through the WordPress GUI at runtime.

## Contact Info

Please contact the Platform Services Team via [Rocket.Chat](https://developer.gov.bc.ca/Steps-to-join-Rocket.Chat) with questions.

## Vendor Info

The code snippets included in this repository were used in a WordPress v5.9.1 instance provided by the [GDX Digital Engagement Solutions team](https://dir.gov.bc.ca/gtds.cgi?show=Branch&organizationCode=CITZ&organizationalUnitCode=GDX%2dDES) using their "Bcgov Engagement" theme v1.1.2.

## Repo Overview

- `./src/additional-css.css`

  - CSS styles that get applied site-wide through the Additional CSS menu (from WP admin panel, Appearance -> Customize -> Additional CSS). This includes styles for components like the Platform Status indicator, which has CSS classes added to it through the WordPress editor GUI (`global-status` and `global-status-up`). Styles like this can be removed as components are built out via custom plugins.

- `./src/alert-banner.html`
  - HTML markup plus a `<style>` block to create an instance of the `warning` style [alert banner from the Design System](https://developer.gov.bc.ca/Design-System/Alert-Banners). This component is a candidate for future development as a custom plugin if we need multiple unique alert banner instances.
