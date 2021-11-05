To do:
Create list of medications
Create list of therapies
Create timeline of therapies in an average CF childs day
Create log in
Create input for therapy and "done"






further app development can be found at: https://github.com/helenbobellon/Cystic_Fibrosis_App


*Sample log in*


def login():    
    user = raw_input("Username: ")
    passw = raw_input("Password: ")
    f = open("users.txt", "r")
    for line in f.readlines():
        us, pw = line.strip().split("|")
        if (user in us) and (passw in pw):
            print "Login successful!"
            return True
    print "Wrong username/password"
    return False

def menu():
    #here's a menu that the user can access if he logged in.

def main():
    log = login()
    if log == True:
         menu()
