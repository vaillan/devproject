# devproject
Using Django inside a Python virtual environment

1. Installing the virtual environment software

  Windows 10 virtual environment setup
    Installing virtualenvwrapper-win is even simpler than setting up virtualenvwrapper because you don't 
    need to configure where the tool stores virtual environment information (there is a default value). 
    All you need to do is run the following command in the command prompt:

    pip3 install virtualenvwrapper-win
    
    Now you can create a new virtual environment with the mkvirtualenv command.
    
2. Creating a virtual environment
  Once you've installed virtualenvwrapper or virtualenvwrapper-win then working with virtual environments is
  very similar on all platforms.
  
  Now you can create a new virtual environment with the mkvirtualenv command. As this command runs
  you'll see the environment being set up (what you see is slightly platform-specific). When the command
  completes the new virtual environment will be active — you can see this because the start of the prompt
  will be the name of the environment in brackets (below we show this for Ubuntu, but the final line is similar
  for Windows/macOS).
  
  The terminal of this example is with linux, you need do it with the cmd of windows 
  
  $ mkvirtualenv my_django_environment
 
  Running virtualenv with interpreter /usr/bin/python3                                           
  ...                                                                                            
  virtualenvwrapper.user_scripts creating /home/ubuntu/.virtualenvs/t_env7/bin/get_env_details   
  (my_django_environment) ubuntu@ubuntu:~$                                                       
  
  Now you're inside the virtual environment you can install Django and start developing.

3. Using a virtual environment
  There are just a few other useful commands that you should know (there are more in the tool documentation, but these are the ones you'll use regularly):
    
    * deactivate — Exit out of the current Python virtual environment
    * workon — List available virtual environments
    * workon name_of_environment — Activate the specified Python virtual environment
    * rmvirtualenv name_of_environment — Remove the specified environment.
    
    For more information go to this link https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/development_environment

4. Create a file for exaple (my_Django_projects) where wass created the virtual environment my_django_environment and download this repository
  
  git clone https://github.com/vaillan/devproject.git
  
  Note.- You need install git for use the commands git clone, or download this file on zip and extract this example of project inside (my_Django_projetcs)

5. Run in your terminal the follows commands:

  * python3 manage.py makemigrations
  * python3 manage.py migrate
  * python3 manage.py createsuperuser # Create a superuser
  * python3 manage.py runserver
  
6.- Open a browser to http://127.0.0.1:8000 to open the admin site
