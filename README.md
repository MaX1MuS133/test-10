from tkinter import *

def hello():
    lbl = Label(text=f'Здравствуйте,{a.get()}!', font=("Consolas", 21, "bold"), foreground='red')
    lbl.place(x=10, y=80)
root=Tk()
root.title('Hello')
root.geometry('500x300')
a = Entry(root, width=10,  bg='white', fg='black', font='consolas')
a.pack()
Button(root, text='Отправить', width=10, height=2, bg='blue',command=hello).pack()
root.mainloop()
