#-*- coding: utf-8 -*-
from tkinter import *  
arr=[
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
   ]
visit=[
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    ]
isalive_flag = 0
#深度优先搜索
def DFS(x, y):
        visit[x][y] = 1 
        directions = [[x - 1, y], [x + 1, y], [x, y - 1], [x, y + 1]] 
        for dx, dy in directions:
                if(dx < 0 or dx > 17 or dy < 0 or dy > 17):
                        continue 
                elif(visit[dx][dy] == 0): 
                        if arr[dx][dy] == 0:
                                global isalive_flag
                                isalive_flag = 1
                                return 
                        elif arr[dx][dy] == - arr[x][y]:
                                continue 
                        elif arr[dx][dy] == arr[x][y]:
                                DFS(dx, dy) 
        return
# 清空搜索记录
def clear_visit():
    global visit
    global isalive_flag
    visit=[
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
    [0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
   ]
    isalive_flag = 0

#有无“气”的判断，有气返回1，无气返回0
def is_alive(x, y):
    isalive = 1 # 用于返回
    clear_visit()
    DFS(x, y)
    # 有“气”标志为0,则返回0,否则为1
    if isalive_flag == 0:
        isalive = 0
    clear_visit()
    return isalive

count=-1
#实现提子操作
def take_out():
    global count
    token_list = [] 
    for i in range(18):
        for j in range(18):
            if(arr[i][j])== 0:
                continue
            elif(arr[i][j]==count and is_alive(i, j) == 0):
                token_list.append([i, j])
    if len(token_list) != 0:        
        for i, j in token_list:
            if(count==1):
                arr[i][j] = -1
                bnt=Button(windows,bg="black",command=lambda x=i, y=j: printc(x, y), height=1,width=3)
                bnt.grid(row=i, column=j) 
            elif(count==-1):
                arr[i][j] = 1
                bnt=Button(windows,bg="white",command=lambda x=i, y=j: printc(x, y),height=1, width=3)
                bnt.grid(row=i, column=j) 

def judge_win():
       global arr
       black=0
       white=0
       for i in range(18):
              for j in range(18):
                     if(arr[i][j]==1):
                            white+=1
                     elif(arr[i][j]==-1):
                            black+=1
       if(black>=162):
              print("black win")
       elif(white>=162): 
              print("white win")
                                                       
def printc(i,j):
        global arr
        global count
        if(count==-1):
                count=1
                arr[i][j]=-1
                bnt=Button(windows,bg="black",command=lambda x=i, y=j: printc(x, y),height=1, width=3)
                bnt.grid(row=i, column=j) 
                take_out()
                judge_win()
        else:
                count=-1
                arr[i][j]=1
                bnt=Button(windows,bg="white",command=lambda x=i, y=j: printc(x, y),height=1, width=3)
                bnt.grid(row=i, column=j)
                take_out() 
                judge_win()
windows=Tk()
windows.geometry("2000x2000")   
windows.title("window") 
#绘制一个名为窗口的窗口并设定大小
for i in range(1,18):
        for j in range(1,18):
                if(arr[i][j]==0):
                        bnt=Button(windows,bg="#ffa000",command=lambda x=i, y=j: printc(x, y),height=1, width=3)
                        bnt.grid(row=i, column=j) 
#利用循环依次建立button绘制成的网格
def printa():
        for i in range(1,18):
                for j in range(1,18):
                        if(arr[i][j]==0):
                               bnt=Button(windows,bg="white",command=lambda x=i, y=j: printc(x, y),height=1, width=3)
                               bnt.grid(row=i, column=j)
                        else:
                                bnt=Button(windows,bg="black",command=lambda x=i, y=j: printc(x, y),height=1, width=3)
                                bnt.grid(row=i, column=j)  

def printb():
        for i in range(1,18):
                for j in range(1,18):
                        if(arr[i][j]==0):
                               bnt=Button(windows,bg="white",command=lambda x=i, y=j: printc(x, y),height=1, width=3)
                               bnt.grid(row=i, column=j) 
                        else:
                                bnt=Button(windows,bg="black",command=lambda x=i, y=j: printc(x, y),height=1, width=3)
                                bnt.grid(row=i, column=j)  
windows.mainloop()

