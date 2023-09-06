# Frappe Bench

Frappe Bench, often referred to as just "Bench," is a command-line tool (CLI) and utility provided by the Frappe framework for managing multiple Frappe applications and instances on a single server. It serves as an essential tool for setting up, configuring, and maintaining Frappe-based applications and is commonly used in development, testing, and production environments.

## Frappe Bench Characteristics

### Installation and Updates

You can use Bench to install and update Frappe and ERPNext (an open-source ERP system built on Frappe). Bench simplifies the process of keeping your applications and the Frappe framework itself up to date.

### Development Environment

Bench is commonly used as part of the development environment for building Frappe applications. Developers can create, test, and customize applications on their local machines and then deploy them to production servers using Bench.

### Site Setup and Configuration

Bench provides commands for setting up new sites, configuring database connections, defining site-specific settings, and managing site backups.

```sh
# To create a new frappe site
bench new-site <site-name>

# To set the site as the default site
bench use <site-name>

# Change site configurations
bench --site <site-name> set-config <config-name> <config-value>

# Clear the site caches
bench --site <site-name> clear-cache
```

### Site Management

Within each Frappe application, Bench can create and manage individual sites. A site represents a specific instance of a Frappe application with its own database and configuration. Sites are useful for hosting multiple independent applications on the same server.

### Application Management

Bench allows you to create, install, and manage multiple Frappe applications on a single server. Each application can have its own configuration, database, and set of installed apps.

```sh
# Create a new custom app
bench new-app <app_name>

# Add the newly custom app to a site
bench --site <site-name> install-app <app-name>

# List all the installed apps on asite
bench --site <site-name> list-apps

# Getting custom apps via github
bench get-app <app-link>

```

### Database Management

Bench offers commands for database management, including database backups, restores, and migrations.

### Logging and Monitoring

You can use Bench to view application and server logs, which is essential for debugging and monitoring the health of your applications.

### Production Deployment

Bench offers deployment commands to set up Frappe applications in production environments, including configuring web servers (e.g., Nginx, Gunicorn), SSL certificates, and more.

## Frappe Bench Project Structure
