# djangocrm

creating the env 




####database sqlite 

python manage.py makemigrations
python manege.py migrate

create the models in the models.py 
#####
    class News(models.Model):
        title = models.CharField(max_length=500)
        body = models.TextField()
        date_posted = models.DateTimeField(auto_now_add=True)

    def __str__(self):
        return self.title
after creating new models

    python manage.py makemigrations

    python manage.py sqlmigrate bloog 0001

    python manege.py migrate
 

