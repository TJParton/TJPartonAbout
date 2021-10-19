# BlockOfCode.md
# Hello, This is some code i did earlier in the semester!

def main():
    
    pi=3.14159
    while (True):
        try:
            radius = float(input('Enter desired radius of cylinder in feet: '))
            if (radius < 0):
                    print('Negtive values for radius are not accepted. ')
                    continue
        except ValueError:
            print('The value you entered is invalid. Only numerical values are valid.' )
        else:
            break
    while (True):
        try:
            height = float(input('Enter desired height of cylinder in feet: ')) 
            if (height < 0):
                    print('Negative values for height are not accepted. ')
                    continue
        except ValueError:
            print('The value you entered is invalid. Only numerical values are valid.')
        else:
            break
    while (True):
        try:
            cost_per_pint = float(input('Enter cost per pint of coating: '))
            if (cost_per_pint < 0):
                    print('Negative values for cost per pint are not accepted. ')
                    continue
        except ValueError:
            print('The value you entered is invalid. Only numerical values are valid.')
        else:
            break
    surface_area = 2 * pi * radius * height + 2 * pi * radius * radius    
    print('The outside surface area of the cylinder in sqft is: ', surface_area)
    number_of_pints = surface_area / 50

    import math
    number_of_pints = math.ceil(number_of_pints)
    print('The number of pints required is: ', number_of_pints)
                  
    cost = number_of_pints * cost_per_pint
    formatted_float = "${:,.2f}".format(cost)
    print('The cost of coating the cylinder is: ', formatted_float)

    restart=input('would you like to perform another calculation? yes or no?').lower()
    if restart == 'yes':
        main()
    else:
        exit()
main()

# Purpose
The point of writing this code was to provide experience with writing an interactive Python program that accepts input, performs a calculation, then displays the result as output while handling invalid input from the user. It also provides experience with loops and controlling them based on user input, exceptions, rounding up values, and formatting output.

At the time when I wrote this I was very proud of myself for being able to do it and I worked very hard to be able to complete the challenge!


# Navigation

*[TJPartonAbout](TJPartonAbout.md)
*[Background](BACKGROUND.md)
*[Things I do](THINGS-I-DO.md)
*[Favorite Music](FAVORITE-MUSIC.md)
*[Favorite Show](FavoriteShows.md)

