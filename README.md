# function1
#program practese with function s in python

def  cyl(h,r):
    area_cyl=2*3.14*r*h
    return area_cyl
def con(l,r):
    area_con=3.14*r*l
    return area_con
#function defination
def post_tax_price(cost):
    tax=0.18*cost
    net_price=cost+tax
    return (net_price)
print("enter values of cylibndrical part of the tent in meters:")
h=float(input("height:"))
r=float(input("radius:"))
csa_cyl=cyl(h,r) #function call
l=float(input("enter slant height:"))
csa_con=con(l,r)
#calculate area of the canvas used for making the tent
canvas_area=csa_cyl+csa_con
print("arae of canvs =",canvas_area,"m^2")
#calculate cost of canvas

#calculate cost of canvs
unit_price=float(input("enter cost of 1 m^s canvs in rupees:"))
total_cost=unit_price*canvas_area
print("total cost of canvas before tax=",total_cost)
print("net amount payble (including tax)=",post_tax_price(total_cost))

#inputs
#h=50
#r=10
#l=20
#units=100

#output
#enter values of cylibndrical part of the tent in meters:
#arae of canvs = 3768.0 m^2
#total cost of canvas before tax= 376800.0
#net amount payble (including tax)= 444624.0

