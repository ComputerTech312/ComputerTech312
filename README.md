### Hello. (•◡•)/

```python
from colby import information

class AboutMe:
    def __init__(self):
        self.name = 'Colby Lipsett'
        self.nick = 'ComputerTech'
        self.birthday = 1028541600
        self.gender = 'male'
        self.about = 'full stack developer/sysadmin that enjoys breaking and fixing things.'
        self.location = 'Ireland'
        self.hobbies = ['Programming', 'Sysadmin', 'IRC', 'LEGO']
        self.languages = ['Python', 'JavaScript', 'Go', 'Tcl']
        self.os = ['Ubuntu']
        self.timezone = ['UTC+1']
        self.projects = [
            {
                'project': 'Sharey',
                'language': 'Python',
                'description': "A website for sharing files, URL redirection and Pastes."
            },
        ]

    def introduce(self):
        print(f'Hello, my name is {self.name}. I\'m from {self.location} and am {self.age} years old.')
        print(f'I\'m a {self.about}.')

my_profile = AboutMe()
my_profile.introduce()

```
