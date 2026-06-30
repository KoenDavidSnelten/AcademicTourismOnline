# Academic Tourism Online

A digital heritage platform built on [Omeka S](https://omeka.org/s/) for exploring and visualising academic tourism collections. The project includes an edited version of the [Freedom theme](https://omeka.org/s/themes/freedom/), styled to follow the visual identity of the University of Groningen (RUG).

## Requirements

- [XAMPP](https://www.apachefriends.org/) (or equivalent Apache + PHP + MySQL stack)
- PHP 8.0+
- MySQL 5.7+ / MariaDB 10.3+

## Modules

| Module | Version |
|--------|---------|
| Omeka S | 4.2.0 |
| ATO Visualisation | 1.0.0 |
| Common | 3.4.86 |
| CSV Import | 2.6.2 |
| Extract Text | 2.1.0 |
| IIIF Presentation | 1.1.2 |
| IIIF Server | 3.6.32 |
| Internationalisation | 3.4.19 |
| Mirador | 3.4.17 |
| Reference | 3.4.62 |
| XML Viewer | 3.4.12 |

## Installation

1. Clone this repository into your web server's document root:
   ```bash
   git clone <repository-url> Academic-Tourism-Online
   ```

2. Copy `config/database.ini.example` to `config/database.ini` and fill in your database credentials.

3. Create a MySQL database for the project and import the provided `.sql` file via phpMyAdmin or the MySQL CLI:
   ```bash
   mysql -u <username> -p <database_name> < database.sql
   ```

4. Place all required modules (listed above) in the `modules/` directory.

5. Open the site in your browser and follow the Omeka S installation wizard.

## Development

This project runs locally via XAMPP. After setup, the site is accessible at:

```
http://localhost/Academic-Tourism-Online
```

The admin interface is available at:

```
http://localhost/Academic-Tourism-Online/admin
```
