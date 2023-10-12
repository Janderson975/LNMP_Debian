Nginx:
  In nginx.conf
  Disabled sevrer tokens
  tls 1.2 and 1.3
  Client timeout
  Request size limits
  Ip whitelist (in readme)
  Enabled sysctl protection x2
  Change user to nginx
  Uncomment pid
  error_log /var/log/nginx/error.log error  
  In sites-available and sites-enabled
  port 443 (in readme)

PostgreSQL:
  In postgressql.conf
  Port 8080 (in readme)
  Turn ssl off
  In conf.d
  Delete envvars
  Delete ports.conf
  In pg_hba.conf
  Change peer to anything else after postgres
  Change peer to anything else after all

  PHP 8.2:
    In php.conf
    Turn engine on
    Turn off short tags
    Turn off asp tags
    Turn off implicit flush
    Set expose php to Off
    Set max execution time to 30
    Set max input time to 60
    Turn of error logging
    Do not ignore repeat errors
    Report memleaks
    Turn on auto_globals_jit
    enable_dl = Off 
    In conf.d
    Remove passwords file

Samba:
  In smb.conf
  obey pam
  browsable set to no
  guest ok set to yes
  



    
