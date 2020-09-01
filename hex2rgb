#!/usr/bin/env python3

import sys

#This is a comment
def rgb_hex():
  invalid_msg = "ERROR: Invalid input"
  red = int(raw_input("Enter Red Value: "))
  
  if red < 0 or red > 255:
    print(invalid_msg)
    return
  
  green = int(raw_input("Enter Green Value: "))
  
  if green < 0 or green > 255:
    print(invalid_msg)
    return
  
  blue = int(raw_input("Enter Blue Value: "))
  
  if blue < 0 or blue > 255:
    print(invalid_msg)
    return
  
  val = (red << 16) + (green << 8) + (blue) 
  
  print("%s" % (hex(val)[2:]).upper())

def hex_rgb(hex_val):
  if len(hex_val) != 6:
    print("ERROR: Invalid value, hex is in 6 characters")
    return
  else: 
    hex_val = int(hex_val, 16)
  
  two_hex_digits = 2 ** 8
  blue = hex_val % two_hex_digits
  hex_val = hex_val >> 8
  green = hex_val % two_hex_digits
  hex_val = hex_val >> 8
  red = hex_val % two_hex_digits
  print("%s\t%s\t%s" % (red,green,blue))
  
def main ():
  with open(sys.argv[1]) as f:
    for l in f.readlines():
      hex_rgb(l.strip())

main()
      
    
  
  
 
