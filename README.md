def hesabla():
    try:
        a = float(input("Birinci rəqəmi daxil edin: "))
        b = float(input("İkinci rəqəmi daxil edin: "))
        emel = input("Əməliyyatı daxil edin (+, -, *, /): ")

        if emel == "+":
            netice = a + b
        elif emel == "-":
            netice = a - b
        elif emel == "*":
            netice = a * b
        elif emel == "/":
            netice = a / b
        else:
            print("Yanlış əməliyyat simvolu daxil edilib.")
            return

        print("Nəticə:", netice)

    except ValueError:
        print("Zəhmət olmasa yalnız ədədi dəyərlər daxil edin.")
    except ZeroDivisionError:
        print("Sıfıra bölmə xətası!")
    except TypeError:
        print("Uyğunsuz tip xətası baş verdi.")
    finally:
        print("Hesablama bitdi.")
