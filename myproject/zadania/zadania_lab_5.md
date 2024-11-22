python manage.py shell
from myapp.models import Person, Team, Stanowisko, Osoba

# 1.
p1 = Person()
>>> p1.name = 'Zosia'
>>> p1.shirt_size = 'M'
>>> p1.age = 13        
>>> p1.save()

p2 = Person()
>>> p2.name = 'Waldek'
>>> p2.shirt_size = 'L'
>>> p2.age = 33        
>>> p2.save()

p3 = Person()
>>> p3.name = 'Waldek'
>>> p3.shirt_size = 'L'
>>> p3.age = 33        
>>> p3.save()




#2
Person.objects.filter(name__startswith='C')

#3.
Person.objects.filter(name__startswith='C').values()