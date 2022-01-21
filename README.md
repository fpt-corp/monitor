# HyperSM Monitor - Cisco SDWAN Demo

A feature demo version of HyperSM - Centralized administration portal made by FIS.

This is the showcase of using Cisco API in integrating with third-party softwares.

![image](https://user-images.githubusercontent.com/49550150/150483861-7a98da02-706a-4710-bc4d-33e35c8031dd.png)

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
    - Click `New`
![image](https://user-images.githubusercontent.com/49550150/150313116-bf878186-a805-4bb0-a8b7-19bd0f5cf216.png)

    - Type name of database (monitor) then click `Create`
![image](https://user-images.githubusercontent.com/49550150/150313285-9d06f3d6-627c-4c02-a4c9-fd84320230c8.png)

    - Choose `monitor` database, click `Import` tab, click `Choose file` and browse to `monitor.sql`, then click `Go` to import database
![image](https://user-images.githubusercontent.com/49550150/150313549-2fd655d4-8627-4cd3-9f56-7ec549c27c62.png)


5. Change file name `env.txt` to `.env`

6. Start `Apache` and `MySQL` service in XAMPP

7. Browse to http://localhost/monitor/public/
    - Click `Generate app key` if RuntimeException page shown (No application encryption key has been specified)
    - Click `Refresh now`

8. Log in with `admin`/`admin`

## Sandbox (Cisco SD-WAN 19.2 Always On)
    https://sandbox-sdwan-1.cisco.com
