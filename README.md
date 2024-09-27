# Persons Module for Odoo

This module implements a simple "Persons" model in Odoo, allowing you to manage personal information, including first name, last name, birthday, age, and sex. It includes automatic calculation of full name and age based on the provided data.

## Features

- Create, read, update, and delete records for persons.
- Automatically compute the full name based on first and last names.
- Automatically compute the age based on the birthday.
- Validation to ensure that the birthday cannot be set in the future.


## Project Setup

### 1. Cloning the Odoo Repository

Clone the project repository:
```shell
git clone https://github.com/AntonKorinchuk/Odoo.git
cd Odoo
```

Clone the Odoo repository into the same directory using the following command:
```shell
git clone https://github.com/odoo/odoo --depth 1 --branch 16.0 --single-branch
```
Create a virtual environment:

```shell
python -m venv venv
```
Activate the virtual environment:
On Windows:
```shell
 venv\Scripts\activate
 ```
On macOS and Linux:
```shell
source venv/bin/activate
```
Install dependencies:
```shell
pip install -r odoo/requirements.txt
```

Rename template_odoo.conf to odoo.conf file and populate it with the required data

Restart the Odoo server:
```shell
odoo/odoo-bin -c conf/odoo.conf
```