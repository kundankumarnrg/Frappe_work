# Frappe_work

Basic Command using frappe_framwork

    >>Create a new bench:
        bench init <bench_name>    # Work with Genral 
        bench init frappe-bench --frappe-branch version-15 --python python3.11    # Work with Frappe V15 and python3.11
        
    >>Create a new bench:
        bench new-site <site_name>
        Enter password

    >>Create a new application:
        bench new-app <app_name>

    >>Install application:
        bench --site code.in install-app <app_name>
        
    >>Set developer mode:
        bench --site <site_name> set-config --global developer_mode 1

    >>Start bench:
        bench start

    >>

    >>


    
Set Internet connection each tab

    >>Connection
        sudo nano /etc/resolv.conf
        nameserver 8.8.8.8 [crel+s, ctrl+x]

How to Start Mairaidb:

    >>Command
        sudo service mariadb start
        

How to install ERPNext on your site

    >>Check ERPNext app avilable or nor
        bench --site inventory.localhost list-apps
    
    >>First, download the ERPNext app in your bench if you haven’t already:
        bench get-app erpnext --branch version-15

    >>Then install ERPNext on your site:
        bench --site inventory.localhost install-app erpnext

    >>After this, run again:
        bench --site inventory.localhost list-apps

    


Clone and install application

    >>You must install it properly. From your bench directory:
        clone repo
        bench get-app maintainx <git_repo_url>

        Install app
        bench --site your-site-name install-app maintainx
      
      
