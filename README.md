# taking-a-vacation
codecademy lesson

def hotel_cost(nights):
    return 140*nights
def plane_ride_cost(city):
    if city == "Charlotte":
        return 183
    elif city == "Tampa":
        return 220
    elif city == "Pittsburgh":
        return 222
    elif city == "Los Angeles":
        return 475
def rental_car_cost(days):
    tickets = days*40 
    if days >= 7:
        tickets += (-50)
    elif days >= 3 and days<7 :
        tickets += (-20)
    return tickets
    #下面trip_cost為什麼只用兩個變數就完成了?hotel的變數為什麼被更改了
def trip_cost(city,days):
    return hotel_cost(days)+plane_ride_cost(city)+rental_car_cost(days)
    #print 要從頭開始寫  
print trip_cost("Los Angeles",5,600)
