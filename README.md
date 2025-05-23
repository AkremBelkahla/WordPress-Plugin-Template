[![Build Status](https://www.travis-ci.org/wpugph/WordPress-Plugin-Template.svg?branch=master)](https://www.travis-ci.org/wpugph/WordPress-Plugin-Template)

WordPress Plugin Template
=========================

A robust and GPL-licensed code template for creating a standards-compliant WordPress plugin.

## Why this template?

This template is the culmination of best practices and lessons learned from developing numerous WordPress plugins. It provides a solid foundation for building high-quality, maintainable plugins.

## How do I use it?

1. Clone this repository or download the files.
2. Run the included build-plugin.sh script to create a new plugin.
3. Follow the prompts to customize the plugin name, destination folder, and Grunt support.

### Running the script

The script will guide you through the process of creating a new plugin. You will be asked to provide:
- **Plugin name**: The full name of your plugin.
- **Destination folder**: The directory where your new plugin will be created.
- **Include Grunt support (y/n)**: Whether to include Grunt files in your new plugin.
- **Initialise new git repo (y/n)**: Whether to initialize a new Git repository in the plugin directory.

### Features

- Plugin headers as required by WordPress & WordPress.org
- Readme.txt file as required by WordPress.org
- Main plugin class
- Full & minified Javascript files
- Grunt.js support for task automation
- Standard enqueue functions for the dashboard and frontend
- Libraries for easily registering new post types and taxonomies
- A versatile settings class for handling plugin options

### API Functions

#### Registering a new post type

Use the post type API to register new post types with ease. Example:
```php
WordPress_Plugin_Template()->register_post_type( 'listing', __( 'Listings', 'wordpress-plugin-template' ), __( 'Listing', 'wordpress-plugin-template' ) );
```

#### Registering a new taxonomy

Use the taxonomy API to register new taxonomies. Example:
```php
WordPress_Plugin_Template()->register_taxonomy( 'location', __( 'Locations', 'wordpress-plugin-template' ), __( 'Location', 'wordpress-plugin-template' ), 'listing' );
```

### Contributing

Contributions are welcome! Please fork this repository and submit a pull request to the `develop` branch. Your contributions will be credited in the changelog.

### License

This project is licensed under the GPLv2 license. See the LICENSE file for details.

## Changelog

See the changelog for a complete list of changes.
