class Student:
    def __init__(self, university):
        self.name = "Gokul Nath"
        self.dob = date(2005, 1, 24)
        self.age = math.floor((date.today() - self.dob).days/365)
        self.lang = ("Tamil", "English")
        self.loc = "Chennai, India"
        self.code_lang = ["Python", "C", "C++", "Java"]
        self.code_framework = ["OpenCV", "Flask", "FastAPI", "discord.py"]
        self.learning = ["Rust", "Django", "TensorFlow"]

    def __str__(self):
        return f"Name: {self.name}\nDoB: {self.dob}\nAge: {self.age}\nLanguage: {', '.join(self.lang)}\nLocation: {self.loc}\nProgramming: {', '.join(self.code_lang)}\nFrameworks: {', '.join(self.code_framework)}\nLearning: {', '.join(self.learning)}"

if __name__ == "__main__":
    import math
    from datetime import date

    me = Student("Sathyabama University")
    print(me)
