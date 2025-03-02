
import tkinter as tk
from tkinter import Tk, Entry, Button, Label , StringVar

window = Tk()
window.geometry("600x250")
window.title("Hausa Dictionary")

entry_text = Entry(window)
entry_text.pack()

result = StringVar()
result_label = Label(window, textvariable=result)
result_label.pack()

hausa_dict = {
               "come" :"zo",
               "go" : "je",
               "father" : "wani",
               "rice" : "shinkafa",
               "fool" : "wawa",
               "home" : "gida",
               "need" : "bukata",
               "again" : "sake",
               "good morning" : "barka da safiya",
               "good afternoon" : "barka da yamma",
               "good bye" : "lafiya lau",
               "good evening" : "barka da yamma",
               "me" : "ni",
               "one" : "daya",
               "two" : "biyu",
               "thank you" : "na gode",
               "stop" : "daina",
               "water" : "ruwa",
               "hello" : "sannu",
               "give me" : "jaara"
}

def hausa(word):
    if word in hausa_dict:
        result.set(hausa_dict[word])
        print(hausa_dict[word])

    else:
        result.set("Not Found")
        print("Not Found")

hausa_btn = Button(window, text= "Hausa", bg="white", fg="blue", padx=20, pady=10, command=lambda: hausa(entry_text.get()))
hausa_btn.pack()

yoruba_dect = {
               "come" : "wa",
               "hello" : "báwo",
               "one" : "mení, ọ̀kan",
               "two" : "méjì",
               "father" : "bàbá",
               "rice" : "ìrẹsì",
               "go" : "lọ",
               "fool" : "Tàn",
               "home" : "Ilé",
               "need" : "ní-lò",
               "again" : "lẹẹkansi",
               "good morning" : "Ẹ kaaro",
               "good afternoon" : "E kaasan",
               "good bye" : "O dabọ",
               "good evening" : "Ẹ ku irole",
               "me" : "Ei",
               "thank you" : "Dúpẹ lọwọ",
               "stop" : "duro",
               "water" : "omi",
               "give me" : "Fun mi"
               }

def Yoruba(word):
    if word in yoruba_dect:
        result.set(yoruba_dect[word])
        print(yoruba_dect[word])

    else: 
         result.set("Not Found")
         print("Not Found")

yoruba_btn = Button(window, text= "Yoruba" , background="white", fg="blue", padx=20, pady=10, command=lambda: Yoruba(entry_text.get()))
yoruba_btn.pack()

Igala_dect = {
              "come" : "Lia ",
              "hello" : "Agba",
              "one" : "oka",
              "two" : "inye",
              "father" : "attah",
              "rice" : "oskapa",
              "go" : "lo",
              "home" : "Ọ̀nọ́",
              "need" : "K'ẹ",
              "again" : "K'ání",
              "good morning" : "Ọ́nwá ọ́nwá",
              "good afternoon" : "Ọ́nwá òwè",              "good bye" : "K'ọ́ nwọ̀",
              "good evening" : "Ọ́nwá ọ́kwu",
              "me" : "Ań",
              "thank you" : "Ọ́nwá ole",
              "stop" : "Kwọ́",
              "water" : "Ọ́mị",
              "give me" : "Na áń"
               }

def Igala(word) :
    if word in Igala_dect:
     result.set(Igala_dect[word])
     print(Igala_dect[word])

    else :
        result>set("Not Found")
        print("Not Found")

Igala_btn = Button(window, text= "Igala", bg="white", fg="blue", padx=20, pady=10, command=lambda: Igala(entry_text.get()))
Igala_btn.pack()  

Igbo_dect = {
             "home" : "Ụlọ",
             "come": "Biá",
             "hello" : "Nnọọ",
             "one" : "Otu",
             "two" : "Abụọ",
             "father" : "Nna",
             "rice" : "Osikapa",
             "go" : "Gaa",
             "home" : "Ụlọ",
             "good morning" : "Ụtụtụ ọma",
             "good afternoon" : "Ehihie ọma" ,
             "water" : "Mmir",
             "again" : "Ọzọ",
             "need" : "Ihe ị",
             "good evening" : "Ehi ọma",
             "me" : "M",
             "thank you" : "Imeela",
             "stop" : "Kwụs",
             "give me" : "Nyefu m"
             }

def Igbo(word):
    if word in Igbo_dect:
        result.set(Igbo_dect[word])
        print(Igbo_dect)

    else :
        result.se("Not Found")
        print("Not Found")

Igbo_btn = Button(window, text= "Igbo", bg= "white", fg="blue", padx=20, pady=10, command=lambda: Igbo(entry_text.get()))
Igbo_btn.pack()

Efik_dect = {
             "hello" : "Mme ndito",
             "come" : "Kpe",
             "home" : "Urua",
             "water" : "Mmin",
             "rice" : "Isip",
             "good bye" : "Uwak mfon",
             "need" : "Kpono",
             "again" : "Kiet",
             "father" : "Ete",
             "one" : "Kiet",
             "two" : "Ibọn̄",
             "give me" : "Nọ mmi",
             "good morning" : "Mme ndito",
             "good evening" : "Mme ndito ke use",
             "good afternoon" : "Mme ndito ke idem",
             "give me" : "Nọ mmi",
             "thank you" : "Sen",
             "go" : "Sua",
             "stop" : "Kada",
             "me" : "Mi"
             }

def Efik(word):
    if word in Efik_dect:
        result.set(Efik_dect[word])
        print(Efik_dect)

    else :
        result.set("Not Found")    
        print("Not Found")


Efik_btn= Button(window, text= "Efik", bg= "white", fg= "blue", padx=20, pady=10, command=lambda: Efik(entry_text.get()))
Efik_btn.pack()        














        
window.mainloop()
