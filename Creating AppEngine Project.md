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
      
      Open a terminal and run this command
      <pre>
      bertopeng17@bertopeng17-ThinkPad-T520:~$ <b>export PATH=$PATH:/home/bertopeng17/go_appengine/</b>
      bertopeng17@bertopeng17-ThinkPad-T520:~$ <b>export PATH=$PATH:/home/bertopeng17/go_appengine/new_project_template</b>
      bertopeng17@bertopeng17-ThinkPad-T520:~$ <b>dev_appserver.py /home/bertopeng17/google_appengine/new_project_template</b>
      </pre>
      <b>Run the command location of the folder / file sample web pages are</b>
      <pre>
      bertopeng17@bertopeng17-ThinkPad-T520:~$ <b>dev_appserver.py /home/bertopeng17/google_appengine/new_project_template/</b>
      Allow dev_appserver to check for updates on startup? (Y/n): y
      dev_appserver will check for updates on startup.  To change this setting, edit /home/bertopeng17/.appcfg_nag
      INFO     2016-03-03 04:29:28,405 sdk_update_checker.py:229] Checking for updates to the SDK.
      INFO     2016-03-03 04:29:28,944 sdk_update_checker.py:257] The SDK is up to date.
      WARNING  2016-03-03 04:29:29,457 simple_search_stub.py:1126] Could not read search indexes from 
      /tmp/appengine.new-project-template.bertopeng17/search_indexes
      INFO     2016-03-03 04:29:29,461 api_server.py:205] Starting API server at: http://localhost:45827
      INFO     2016-03-03 04:29:29,475 dispatcher.py:197] Starting module "default" running at: http://localhost:8080
      INFO     2016-03-03 04:29:29,478 admin_server.py:116] Starting admin server at: http://localhost:8000
      INFO     2016-03-03 04:29:38,370 module.py:787] default: "GET / HTTP/1.1" 200 12
      INFO     2016-03-03 04:29:38,449 module.py:787] default: "GET /favicon.ico HTTP/1.1" 200 8348
      INFO     2016-03-03 04:29:38,514 module.py:787] default: "GET /favicon.ico HTTP/1.1" 304 -
      </pre>
      
      then open the url and type <b>http: // localhost: 8080 / </b>  if true it will show a "hello world"
      
      To upload these pages in google appengine, you must register in advance at http://appengine.google.com/, When you're able       to open new tabs in the terminal, because of previous orders not in close, if at the close eating localhost will die. Run       this command back
      
      <pre>
     bertopeng17@bertopeng17-ThinkPad-T520:~$ <b>dev_appserver.py /home/bertopeng17/google_appengine/</b>
     bertopeng17@bertopeng17-ThinkPad-T520:~$ <b>dev_appserver.py /home/bertopeng17/google_appengine/new_project_template</b>
     INFO     2016-03-03 05:12:23,687 sdk_update_checker.py:229] Checking for updates to the SDK.
     INFO     2016-03-03 05:12:24,140 sdk_update_checker.py:257] The SDK is up to date.
     INFO     2016-03-03 05:12:24,220 api_server.py:205] Starting API server at: http://localhost:55478
     INFO     2016-03-03 05:12:24,226 api_server.py:648] Applying all pending transactions and saving the datastore
     INFO     2016-03-03 05:12:24,226 api_server.py:651] Saving search indexes
     Traceback (most recent call last):
      File "/usr/local/google_appengine/dev_appserver.py", line 83, in <module>
    _run_file(__file__, globals())
     File "/usr/local/google_appengine/dev_appserver.py", line 79, in _run_file
    execfile(_PATHS.script_file(script_name), globals_)
    File "/usr/local/google_appengine/google/appengine/tools/devappserver2/devappserver2.py", line 1040, in <module>
    main()
   File "/usr/local/google_appengine/google/appengine/tools/devappserver2/devappserver2.py", line 1033, in main
    dev_server.start(options)
   File "/usr/local/google_appengine/google/appengine/tools/devappserver2/devappserver2.py", line 824, in start
    self._dispatcher.start(options.api_host, apis.port, request_data)
  File "/usr/local/google_appengine/google/appengine/tools/devappserver2/dispatcher.py", line 194, in start
    _module.start()
  File "/usr/local/google_appengine/google/appengine/tools/devappserver2/module.py", line 1176, in start
    self._balanced_module.start()
  File "/usr/local/google_appengine/google/appengine/tools/devappserver2/wsgi_server.py", line 315, in start
    self._start_all_fixed_port(host_ports)
  File "/usr/local/google_appengine/google/appengine/tools/devappserver2/wsgi_server.py", line 352, in _start_all_fixed_port
    raise BindError('Unable to bind %s:%s' % self.bind_addr)
   google.appengine.tools.devappserver2.wsgi_server.BindError: Unable to bind localhost:8080
   bertopeng17@bertopeng17-ThinkPad-T520:~$ 
</pre>

to complette tutorial please click url : https://cloud.google.com/appengine/docs/python/
