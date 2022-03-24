from tkinter import *
from tkinter.ttk import *
from time import strftime

root = Tk()
root.title("watch")
def time():
    string=strftime('%H:%M:%S:%p')
    label.config(text=string)
    label.after(1000,time)
label = Label(root, font=("DS-DİGİ.TTF",80),background="white",foreground="purple")
label.pack(anchor="center")
time()
mainloop()
