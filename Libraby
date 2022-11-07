class Library:
    
    def __init__(self, ListOfBook):
        self.books = ListOfBook

    def AvailableBooks(self):
     for book in self.books:
        print(" *"+ book)

    def borrowbook(self,bookname ):
        if bookname in self.books:
            print(f"you have been issued {bookname} book , please keep it properly and return it on time !")
            self.books.remove(bookname)
            return True        
        else :
         print("sorry this book has already issued to someone else !") 
         return False
         
    def returnbook(self,borrowname):
        self.books.append(borrowname)
        print("thanks for returning this book, have a nice day ahead! ")

class student:

    def reqbook(self):
        self.book = input("Enter the book name that you want to borrow :")
        return self.book

    def returnbook(self):
        self.book = input("Enter the book name that you want to return :")
        return self.book    

if __name__ == "__main__":
    centrallibrary = Library(["english","nowel", "maths", "biology", "history"]) 
    Student = student()
    while(True):
        welcomeMSG = '''======Welcome To  Central Library======
        Please choose an option :

        1.Listing all the books
        2.Borrow a book
        3.Return a book 
        4.Exit()        
        '''
        print(welcomeMSG)
        a =int(input("Enter a choice :"))
        if a==1:
            centrallibrary.AvailableBooks()

        elif a == 2 :
            centrallibrary.borrowbook(Student.reqbook())
        elif a ==3 :
            centrallibrary.returnbook(Student.returnbook())
        elif a ==4:
            print("thanks for using it have a great day !")
            exit()
        else :
            print("Invalid choice !")
