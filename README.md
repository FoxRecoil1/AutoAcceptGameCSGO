#AutoAcceptGameCSGO
import mouse
import time
import pyautogui
run = True
runinf = True
lang = 0
ra = 0
run = True
while run:
    try:
        print("Language? (In game)")
        print("1 English\Английский")
        print("2 Русский\Russian")
        num = int(input("Send Number: "))
        if num == 1:
            lang = 1
            print("")
            print("English")
            print("")
            run = False
            time.sleep(2)
        if num == 2:
            lang = 2
            print("")
            print("Русский")
            print("")
            run = False
            time.sleep(2)
        if num != 1 and num != 2:
            print("")
            print("Send Number!")
            print("")
            run = True
    except NameError:
        print("Send Number!")
    except SyntaxError:
        print("Send Number!")
run = True
while run:
    try:
        if lang == 1:
            print("")
            print("Select the game screen coloring!")
            print("")
            print("1. 16|9 or 16|10")
            print("2. 4|3")
            print("")
            num = int(input("Send Number: "))
            if num == 1:
                ra = 1
                print("")
                print("16|9 or 16|10")
                print("")
                run = False
                time.sleep(2)
            if num == 2:
                ra = 2
                print("")
                print("4|3")
                print("")
                run = False
                time.sleep(2)
            if num != 1 and num != 2:
                print("")
                print("Send Number!")
                print("")
                run = True
        if lang == 2:
            print("")
            print("Выберите разрешение экрана КС:ГО")
            print("")
            print("1. 16|9 или 16|10")
            print("2. 4|3")
            print("")
            num = int(input("Ввидите число: "))
            if num == 1:
                ra = 1
                print("")
                print("16|9 или 16|10")
                print("")
                run = False
                time.sleep(2)
            if num == 2:
                ra = 2
                print("")
                print("4|3")
                print("")
                run = False
                time.sleep(2)
            if num != 1 and num != 2:
                print("")
                print("Напиши Число!")
                print("")
                run = True

    except NameError:
        print("Send Number!")
    except SyntaxError:
        print("Send Number!")
try:
    if ra == 1 and lang == 1:
        runinf = True
        while runinf:
            start = pyautogui.locateCenterOnScreen("Accept1900Eng.png", confidence=0.3)
            print(start)
            if start != None:
                pyautogui.moveTo(start)
                mouse.click("left")
                print("The button is captured the mission is completed!")
                runinf = False
                time.sleep(10)
                break
    if ra == 1 and lang == 2:
        runinf = True
        while runinf:
            start = pyautogui.locateCenterOnScreen("Accept1900Rus.png", confidence=0.3)
            print(start)
            if start != None:
                pyautogui.moveTo(start)
                mouse.click("left")
                print("Кнопка Захваченна миссия выполненна!")
                runinf = False
                time.sleep(10)
                break
    if ra == 2 and lang == 1:
        runinf = True
        while runinf:
            start = pyautogui.locateCenterOnScreen("Accept1300Eng.png", confidence=0.3)
            print(start)
            if start != None:
                pyautogui.moveTo(start)
                mouse.click("left")
                print("The button is captured the mission is completed!")
                runinf = False
                time.sleep(10)
                break
    if ra == 2 and lang == 2:
        runinf = True
        while runinf:
            start = pyautogui.locateCenterOnScreen("Accept1300Rus.png", confidence=0.3)
            print(start)
            if start != None:
                pyautogui.moveTo(start)
                mouse.click("left")
                print("Кнопка Захваченна миссия выполненна!")
                runinf = False
                time.sleep(10)
                break
except NameError:
    print("Send Number!")
except SyntaxError:
    print("Send Number!")


