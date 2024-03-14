### Hello. (•◡•)/

```python
from colby import information

class AboutMe:
    def __init__(self):
        self.name = 'Colby'
        self.user = 'ComputerTech'
        self.age = 1028541600
        self.gender = 'male'
        self.about = 'full stack developer/sysadmin that enjoys breaking and fixing things.'
        self.birth_country = 'Ireland'
        self.location = 'Warsaw, Poland'
        self.hobbies = ['Programming', 'Sysadmin', 'IRC', 'LEGO']
        self.languages = ['Python', 'HTML', 'CSS', 'JavaScript', 'Go', 'Tcl', 'C', 'C++']
        self.os = ['Ubuntu', 'FreeBSD', 'Windows']
        self.timezone = ['UTC+1']
        self.projects = [
            {
                'project': 'elitebot',
                'language': 'Python',
                'description': "This is a Python-based IRC bot that is simple and doesn't use any third-party frameworks."
            },
        ]

    def introduce(self):
        print(f'Hello, my name is {self.name}. I\'m from {self.location} and {self.age} years old.')
        print(f'I was born in {self.birth_country} and currently live in {self.current_country}.') 
        print(f'I\'m a {self.about}.')

my_profile = AboutMe()
my_profile.introduce()

```
