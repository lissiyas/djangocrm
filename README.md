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


go the python shell
        
        python manage.py shell
        from mars.models import Publication  #import the model 
        Publication.objects.all()  #to querry all the data in the model
        publication_1 = Publication(title = 'securing noc using incremental cryptogaphy', author ='lissiyas Antony' , body ='published in the ISQUED') #create the sample data
        publication_1.save()

after that register that model in admin page

        from .models import News , Publication
        
        admin.site.register(News)
        admin.site.register(Publication)

