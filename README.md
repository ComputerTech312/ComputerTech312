### Hello. 👋

```python
from colby import information

class AboutMe:
    def __init__(self):
        self.name = 'Colby'
        self.user = 'ComputerTech'
        self.age = 21
        self.gender = 'male'
        self.about = 'full stack developer/sysadmin that enjoys breaking and fixing things.'
        self.location = 'Ireland'
        self.hobbies = ['Programming', 'Sysadmin', 'IRC', 'LEGO']
        self.languages = ['Python', 'Go', 'HTML', 'CSS', 'Javascript', 'TCL']
        self.os = ['Ubuntu', 'FreeBSD']
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
        print(f'Hello, my name is {self.name} from {self.location}, {self.age} years old {self.gender}. I was born on {self.formatted_dob}. I am a {self.about}')

my_profile = AboutMe()
my_profile.introduce()

```
