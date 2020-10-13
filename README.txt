This simple tiny app helps users to maintain notes on github.


HOW TO USE IT...?

1.Create a Django project using:
django-admin startproject projectname

2. cd into project folder using:
cd projectname

3. Install techynotes app in your django project using:
pip install techynotes

4. In settings.py add techynotes in INSTALLED_APPS

INSTALLED_APPS=[
...
'techynotes',
...
]

5. Include techynotes url in your project urls.py

urlpatterns = [
    ...
    
    url(r'^notes/', include('techynotes.urls')),
    
    ...
    ]
    
    
    6. Now you have successfully configured the techynotes app in your django project, so finally you can run your django server using:
    python3 manage.py runserver
    
    and you can visit this url :  http://127.0.0.1:8000/notes/
    
    
    7. You should able to see the UI, where you can login to start writting and saving your notes on github, or you can search for any other users notes by just entering their git username in the search bar.
    
    Example, you can seach for 'kom3' (my git username).
    
    It will list all the available notes and you can click on any of the note to open it.
