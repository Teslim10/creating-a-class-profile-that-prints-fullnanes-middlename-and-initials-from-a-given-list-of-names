# creating-a-class-profile-that-prints-fullnanes-middlename-and-initials-from-a-given-list-of-names
'''We have the profiles (first name, middle name, last name) of all registered users on a website written to a variable 'users' as:
users = """Olalade John Adewole
Alimat Faizah Suleman
Ekene James Benson"""
(Notice that the profiles are separated by the line break \n character)
We need to extract only parts of these names for any specified user. (Users are specified by indices 1 - 3).
Write a class named 'profile' that gives the first name, middle name, last name, initials or full name of any of the users.
After creating the class, append your code with the following lines of code:
➖➖➖➖➖➖➖➖➖➖➖
user1 = profile(1)
user2 = profile(2)
user3 = profile(3)
print(user1.user)
print(user2.first)
print(user3.initials)
➖➖➖➖➖➖➖➖➖➖➖
Your output should be:
➖➖➖➖➖➖➖➖➖➖➖
Olalade John Adewole
Alimat
EJB
>>>
➖➖➖➖➖➖➖➖➖➖➖'''
users = """Olalade John Adewole
Alimat Faizah Suleman
Ekene James Benson"""

class profile :
	def __init__ (self, y):
		User_List = users.split("\n")
		if y == 1:
			self.y = User_List[0]
		if y == 2:
			self.y = User_List[1]
		if y == 3:
			self.y = User_List[2]
	def user (self):
		return self.y
	def firstname (self):
		Name = self.y.split(" ")
		Firstname = Name [0]
		Middlename = Name [1]
		Lastname = Name [2]
		return Firstname
	def middlename (self):
		Name = self.y.split(" ")
		Firstname = Name [0]
		Middlename = Name [1]
		Lastname = Name [2]
		return Middlename
	def lastname (self):
		Name = self.y.split(" ")
		Firstname = Name [0]
		Middlename = Name [1]
		Lastname = Name [2]
		return Lastname
	def initials (self):
		Name = self.y.split(" ")
		Firstname = Name [0]
		Middlename = Name [1]
		Lastname = Name [2]
		return Firstname[0]+Middlename[0]+Lastname[0]
user1 = profile(1)
user2 = profile(2)
user3 = profile(3)

print(user1.user())
print(user2.firstname())
print(user3.initials())
                   
