This Module return back an excel file including all controlling switches and parameters related to Huawei LTE PDCCH package.

1- on Huawei OSS , export LTE base Station Bulk configuration 
2- Bulk file needs to have following MOs:
----------CELL
----------CELLALGOSWITCH
----------CELLDLPCPDCCH
----------CELLPDCCHALGO

3- if bulk configuration has more MOs rather than what was mentioned in step 2 , it is OK ,No Need To remove
4- Paste exported bulk file in same directory as ANR.Exe file.Please don't change anything inside bulk file.
5- change name of bulk file to "Config"
6- Double click on PDCCH.Exe , wait for Output which is an excel file 
