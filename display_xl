#!/usr/local/bin/python
import xlrd, sys 

try:
        book = xlrd.open_workbook(sys.argv[1])
except IndexError:
        print "Error: Need to parse a file"
        sys.exit()
except IOError:
        print "Error: Cannot find file"
        sys.exit()

for sheet in book.sheets():
    print sheet.name
    for rx in range(sheet.nrows):
        for cx in range(sheet.ncols):
            print sheet.cell_value(rx,cx), "\t",
        print "\n",
    print "\n"
