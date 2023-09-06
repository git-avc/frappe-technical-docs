# Frappe Sites Introduction

In Frappe, a "site" refers to a specific instance or installation of a Frappe application. Each site represents a separate environment where a Frappe-based application is deployed and run. Sites are used to isolate different instances of applications, allowing multiple applications to be hosted on a single server or infrastructure while keeping their data and configurations separate.

## Frappe sites characteristics

### Isolation

Sites provide isolation at the database and configuration levels. Each site has its own database where data is stored and its own configuration settings, including customizations, settings, and installed apps.

### Multitenancy

Frappe supports a multitenant architecture, which means you can host multiple independent applications or tenants on a single Frappe instance. Each tenant corresponds to a separate site.

### Configuration

Each site has its own configuration file (`sites/{site_name}/site_config.json`) where you can define settings specific to that site, such as database connection details, email settings, and custom app configurations.

### App Installation

Apps can be installed on a per-site basis. This allows you to install different sets of apps for different sites. Each site can have its own set of enabled apps.

### Customizations

Customizations, including custom DocTypes, fields, scripts, and templates, can be applied to a specific site without affecting other sites.

### Domain and Host Mapping

Sites can have their own domain names or subdomains, allowing you to run multiple sites on a single server with different URLs. For example, "site1.example.com" and "site2.example.com" can point to different Frappe sites.

### Site-Specific Assets

Each site can have its own assets, such as static files, templates, and uploaded media, which are separate from those of other sites.

## Frappe site 