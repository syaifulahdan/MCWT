### MCWT - Mobile Computing and Web Technologies

   Creating a new Project
   please access the following url : http://console.developer.google.com
   please enter Projec name and project id (automaticaly) for example : 
   projec name : bertopeng17
   project id  : bertopeng17-1238  ( project id will be filled in automatically)



  Intro to Exercises Development Environment Code Repo
    -  goals : learn how to write endpoints functions
    -  Use the APIs Explorer
    -  get started started with the app confrence central app
    
   the tools you'll need
   -  text editor - a programming text editor
   -  python - 2.7 - use python --version  to check
   -  git - control software
   -  google app engine SDK
   

   - tex editor : The default text editor can use in the operating system, for example: linux: gedit, or install 
      <pre>
      $sudo apt-get install gedit
      </pre>

   -  python can use default in operating system ubuntu
      <pre>
      bertopeng17@bertopeng17-ThinkPad-T520:~$ python
      Python 2.7.6 (default, Jun 22 2015, 18:00:18) 
      [GCC 4.8.2] on linux2
      Type "help", "copyright", "credits" or "license" for more information.
      >>> 
      </pre>
   -  git can install your system via terminal
      <pre>
      bertopeng17@bertopeng17-ThinkPad-T520:~$ sudo apt-get install git-all
      </pre>

   - Google app engine SDK : https://cloud.google.com/appengine/downloads#Google_App_Engine_SDK_for_Python
     or directly download on url : https://storage.googleapis.com/appengine-sdks/featured/google_appengine_1.9.33.zip
      
      <b>Setup Google App Engine Python SDK in Ubuntu</b>
      Extract it anywhere within your local folder. It can be anywhere such as in your home directory or Documents directory.
      Open terminal (ctrl+alt+t) and navigate to your home directory and open .bashrc to edit with this command:
      <pre>
      $ sudo gedit .bashrc
      </pre>

      At the end of the file, add these lines by changing the directory to your google_appengine folder. The first line is just       a comment and in the second line /usr/local/google_appengine is the path to the google_appengine folder.
      <pre>
      ### Added for GAE
      export PATH="/usr/local/google_appengine:$PATH"
      </pre>
      
      Now restart your computer and then you should be able to use <b>$ dev_appserver.py </b> command from anywhere
      <pre>
      bertopeng17@bertopeng17-ThinkPad-T520:~$ <b>dev_appserver.py</b>
      usage: dev_appserver.py [-h] [-A APP_ID] [--host HOST] [--port PORT]
                        [--admin_host ADMIN_HOST] [--admin_port ADMIN_PORT]
                        [--auth_domain AUTH_DOMAIN] [--storage_path PATH]
                        [--log_level {debug,info,warning,critical,error}]
                        [--max_module_instances MAX_MODULE_INSTANCES]
                        [--use_mtime_file_watcher [USE_MTIME_FILE_WATCHER]]
                        [--threadsafe_override THREADSAFE_OVERRIDE]
                        [--php_executable_path PATH]
                        [--php_remote_debugging [PHP_REMOTE_DEBUGGING]]
                        [--php_gae_extension_path PATH]
                        [--php_xdebug_extension_path PATH]
                        [--appidentity_email_address APPIDENTITY_EMAIL_ADDRESS]
                        [--appidentity_private_key_path APPIDENTITY_PRIVATE_KEY_PATH]
                        [--python_startup_script PYTHON_STARTUP_SCRIPT]
                        [--python_startup_args PYTHON_STARTUP_ARGS]
                        [--jvm_flag JVM_FLAG]
                        [--custom_entrypoint CUSTOM_ENTRYPOINT]
                        [--runtime RUNTIME] [--blobstore_path BLOBSTORE_PATH]
                        [--mysql_host MYSQL_HOST] [--mysql_port MYSQL_PORT]
                        [--mysql_user MYSQL_USER]
                        [--mysql_password MYSQL_PASSWORD]
                        [--mysql_socket MYSQL_SOCKET]
                        [--datastore_path DATASTORE_PATH]
                        [--clear_datastore [CLEAR_DATASTORE]]
                        [--datastore_consistency_policy {consistent,random,time}]
                        [--require_indexes [REQUIRE_INDEXES]]
                        [--auto_id_policy {sequential,scattered}]
                        [--logs_path LOGS_PATH]
                        [--show_mail_body [SHOW_MAIL_BODY]]
                        [--enable_sendmail [ENABLE_SENDMAIL]]
                        [--smtp_host SMTP_HOST] [--smtp_port SMTP_PORT]
                        [--smtp_user SMTP_USER]
                        [--smtp_password SMTP_PASSWORD]
                        [--smtp_allow_tls [SMTP_ALLOW_TLS]]
                        [--prospective_search_path PROSPECTIVE_SEARCH_PATH]
                        [--clear_prospective_search [CLEAR_PROSPECTIVE_SEARCH]]
                        [--search_indexes_path SEARCH_INDEXES_PATH]
                        [--clear_search_indexes [CLEAR_SEARCH_INDEXES]]
                        [--enable_task_running [ENABLE_TASK_RUNNING]]
                        [--allow_skipped_files [ALLOW_SKIPPED_FILES]]
                        [--api_port API_PORT]
                        [--automatic_restart [AUTOMATIC_RESTART]]
                        [--dev_appserver_log_level {debug,info,warning,critical,error}]
                        [--skip_sdk_update_check [SKIP_SDK_UPDATE_CHECK]]
                        [--default_gcs_bucket_name DEFAULT_GCS_BUCKET_NAME]
                        yaml_path [yaml_path ...]
      dev_appserver.py: error: too few arguments
      bertopeng17@bertopeng17-ThinkPad-T520:~$ 

      </pre>
      
to complette tutorial please click url : https://cloud.google.com/appengine/docs/python/
