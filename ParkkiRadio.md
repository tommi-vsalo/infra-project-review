# ParkkiRadio

## Project Overview
The ParkkiRadio project seeks to track parking lot activity with that car tyre pressure sensor radio signals. The end result was a dashboard that displays the situation in parking locations in accordance with the data.

Due to the nature of the project, I couldn't test it in action. The repository itself didn't have concrete results of the system in action, but I will still review the operating principles.

### Components

The project consisted of:

- Webserver
- Database server
- Sensor
- Cloud hosted dashboard

### Operating Principles

In theory, the project works by sending captured TPMS sensor data through the webserver into the database server. Both servers are cloud hosted and feed the data into the dashboard.

## Project Review

The project incorporated many different features and technologies. The project required skills in server management, several domain specific languages and a good understanding of how the sensors work. The pipeline from data acquisition --> data transfer --> data processing --> data display is quite impressive.

The project portfolio could use evidence of the project in action. The repository mentions several issues with the sensors including inconsistent transmitting, difficulties in identifying sources, the type of detection zone etc. It also acknowledges that these make the system only advisory. This could still be highly useful regardless of the difficulties, but as of now I can't tell how reliable the base functions were either.
