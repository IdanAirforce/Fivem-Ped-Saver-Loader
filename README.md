Ped Saver with Real-Time Replacement in SQL

This FiveM script allows players to save their ped models in an SQL database and replace them in real time through commands and a menu.

Features

Save a player's ped model to the database.

Replace the player's ped model in real time.

Reset to a default ped model.

Retrieve saved ped models via a client-side menu.

Installation

Database Setup:
Create a table in your database:

CREATE TABLE idan_peds (
    id INT AUTO_INCREMENT PRIMARY KEY,
    identifier VARCHAR(255) NOT NULL,
    model VARCHAR(255) NOT NULL
);

Configure the Default Ped:
In the client script, set your default ped model:

Config = {
    defaultPedModel = "a_m_y_stbla_01"
}

Add to Server Config:
Add this resource to your server.cfg:

start idan-savepeds

Usage

Use /addped [model] to save a ped model.

Use /savedpeds to open the menu and view saved peds.

License

This project is licensed under the MIT License.
