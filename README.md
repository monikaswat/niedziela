# niedziela


def passwd_length(passwd):
    print(f'Dlugosc hasla: {len(passwd)}')
    return len(passwd)


def user_exist(user):
    if user in users.keys():
        return True

 def passwd_correct(name, passwd):
    if users[name] == passwd:
        return True
    return False
users = {
    'Monika': 'Monika1',
    'Doris': 'Mandarynka',
    'Kasia_python': 'Python0'
}


------

def net_salary(age, gross_salary=3000, year=2024):
    if age < 26:
        return f'w roku {year} wyplata wynosi {gross_salary}'
    else:
        return f'w roku {year} wyplata wynosi {gross_salary *.8}'

print(net_salary(year=2021, age=5000))
print(net_salary(43, 100))

-------



class Czlowiek:
    def __init__(self, id, name):
        self.id = id
        self.name = name
        self.mail = name+'@firma.com'
        self.urlop = 15

pracownik1 = Czlowiek(999, 'Marek')
print(pracownik1.name)
print(pracownik1.urlop)
pracownik1.urlop = 20
print(Czlowiek)



-----


class Czlowiek:
    def __init__(self, id, name):
        self.id = id
        self.name = name
        self.mail = name+'@firma.com'
        self.urlop = 15

    def wykorzystaj_urlop(self, ile):
        if self.urlop >= ile:
            self.urlop -= ile
        else:
            pritn('Brak urlopu')


