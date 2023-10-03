### Hello. 👋

```python
from datetime import datetime

class AboutMe:
    def __init__(self):
        self.name = 'Colby'
        self.user = 'ComputerTech'
        self.dob = 1028548800
        self.gender = 'male'
        self.about = 'full stack developer/sysadmin that enjoys breaking and fixing things.'
        self.location = 'Ireland'
        self.hobbies = ['Programming', 'Sysadmin', 'IRC']
        self.languages = ['Python', 'Go', 'HTML', 'CSS', 'Javascript', 'TCL']
        self.os = ['Ubuntu', 'Debian', 'Windows']
        self.timezone = ['UTC+1']
        self.projects = [
            {
                'project': 'elitebot',
                'language': 'Python',
                'description': "This is a Python-based IRC bot that is simple and doesn't use any third-party frameworks."
            },
            {
                'project': 'ninjawall',
                'language': 'Python',
                'description': "A user-friendly utility that optimizes the manipulation of iptables for efficient management of network traffic."
            },
        ]

        self.calculate_age()

    def calculate_age(self):
        dob_datetime = datetime.fromtimestamp(self.dob)
        current_datetime = datetime.now()
        age_timedelta = current_datetime - dob_datetime
        self.age = age_timedelta.days // 365

    def introduce(self):
        print(f'Hello, my name is {self.name} from {self.location}, {self.age} years old {self.gender}. I was born on {self.formatted_dob}. I am a {self.about}')

    @property
    def formatted_dob(self):
        return f"{datetime.fromtimestamp(self.dob):%d-%m-%Y}"

my_profile = AboutMe()
my_profile.introduce()

```
