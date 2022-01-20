# HyperSM Monitor - Cisco SDWAN Demo

A feature demo version of HyperSM - Centralized administration portal made by FIS.

This is the showcase of using Cisco API in integrating with third-party softwares.

## Prerequisite

* XAMPP
* Composer

## Installation

1. Change folder name from `monitor-main` to `monitor` if needed then copy `monitor` folder to `C:\xampp\htdocs`

2. Enable SOAP: edit file `C:\xampp\php\php.ini`
```sh
#from
;extension=soap
#to
extension=soap
```

3. Update composer (open cli and navigate to `monitor` folder)
```sh
composer update
```

4. Create `monitor` database (in `phpmyadmin`) then import file `monitor.sql`

5. Change file name `env.txt` to `.env`

6. Start `Apache` and `MySQL` service in XAMPP

7. Browse to http://localhost/monitor/public/
    - Click `Generate app key` if RuntimeException page shown (No application encryption key has been specified)
    - Click `Refresh now`

8. Log in with `admin`/`admin`

## Sandbox (Cisco SD-WAN 19.2 Always On)
    https://sandbox-sdwan-1.cisco.com
