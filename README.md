### Hello. (•◡•)/

```python
from colby import information

class AboutMe:
    def __init__(self):
        self.name = 'Colby'
        self.user = 'ComputerTech'
        self.age = 21
        self.gender = 'male'
        self.about = 'full stack developer/sysadmin that enjoys breaking and fixing things.'
        self.birth_country = 'Ireland'
        self.location = 'Warsaw, Poland'
        self.hobbies = ['Programming', 'Sysadmin', 'IRC', 'LEGO']
        self.languages = ['Python', 'HTML', 'CSS', 'Javascript', 'Tcl']
        self.os = ['Ubuntu', 'FreeBSD', 'Windows']
        self.timezone = ['UTC+0']
        self.projects = [
            {
                'project': 'elitebot',
                'language': 'Python',
                'description': "This is a Python-based IRC bot that is simple and doesn't use any third-party frameworks."
            },
            {
                'project': 'tilde.green',
                'url': 'https://tilde.green',
                'description': "tilde.green is an open community that thrives of creativity and wildness"
            },
        ]

    def introduce(self):
        print(f'Hey, how's it going?, my name is {self.name} from {self.location}, {self.age} years old {self.gender}. I was born in {self.birth_country} and currently live in {self.current_country}. I am a {self.about}')

my_profile = AboutMe()
my_profile.introduce()

```
