- 👋 Hi, I’m @MmdmoSav
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
MmdmoSav/MmdmoSav is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
M='raised'
L='#007a33'
K='#c8102e'
J='Oman IPv4 Generator'
F='#ffffff'
E='Arial'
import tkinter as C,random as G,ipaddress as A
N=[A.ip_network('185.27.88.0/22'),A.ip_network('185.29.140.0/22'),A.ip_network('185.53.240.0/22'),A.ip_network('185.64.24.0/22'),A.ip_network('185.69.0.0/24'),A.ip_network('185.112.104.0/22'),A.ip_network('185.123.148.0/22'),A.ip_network('185.143.64.0/22'),A.ip_network('185.186.204.0/22'),A.ip_network('185.226.124.0/22'),A.ip_network('185.233.168.0/22'),A.ip_network('185.255.204.0/22'),A.ip_network('188.65.24.0/21')]
def O():A=G.choice(N);B=str(G.choice(list(A.hosts())));return B
def P():A=O();D.delete(0,C.END);D.insert(0,A);D.icursor(C.END)
def Q():A=D.get();B.clipboard_clear();B.clipboard_append(A);B.update();D.delete(0,C.END);D.insert(0,'Copy is done')
B=C.Tk()
B.title(J)
H=400
I=300
R=B.winfo_screenwidth()
S=B.winfo_screenheight()
T=R/2-H/2
U=S/2-I/2
B.geometry(f"{H}x{I}+{int(T)}+{int(U)}")
B.configure(bg=K)
D=C.Entry(B,width=30,font=(E,16),justify='center',bg=F,fg='#000000')
D.pack(pady=20)
V=C.Button(B,text=J,command=P,font=(E,14),bg=L,fg=F,relief=M)
V.pack(pady=10)
W=C.Button(B,text='Copy to Clipboard',command=Q,font=(E,14),bg=L,fg=F,relief=M)
W.pack(pady=10)
X=C.Label(B,text='Made by: t.me/HELLBoY_shop\nLocation: Oman',font=(E,12),bg=K,fg=F)
X.pack(side='bottom',pady=10)
B.mainloop()
