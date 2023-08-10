This tools is provided to compare PCI / TAC / ARFCN of EUTRANEXTERNALCELL MO to CELL MO & CNOPERATORTA MO
and find if there is any discrepancy and mis-configuration .

1- on Huawei OSS , export LTE base Station Bulk configuration 
2- Bulk file needs to have following MOs:
----------CELL
----------EUTRANEXTERNALCELL
----------CNOPERATORTA

3- if bulk configuration has more MOs rather than what was mentioned in step 2 , it is OK ,No Need To remove
4- Paste exported bulk file in same directory as EXTCell.exe file.Please don't change anything inside bulk file.
5- change name of bulk file to "Config"
6- Double click on EXTCell.exe , wait for Output which is an excel file named NBR_EXT
7- in NBR_EXT there is a column entitled "Mismatch_Columns" which shows discrepancies.you may see one of following options
------------------- PCI : just PCI is different
------------------- TAC : just TAC is different
------------------- ARFCN : just ARFCN is different
------------------- PCI + TAC : PCI and TAC are different in two MOs
------------------- PCI + ARFCN : PCI and ARFCN are different in two MOs
------------------- TAC + ARFCN : ARFCN and TAC are different in two MOs
------------------- TAC + PCI + ARFCN : PCI and TAC and ARFCN are different in two MOs
------------------- No_Data_In_Database : No match was found CELL MO associated with eNB ID + Cell ID configured in EUTRANEXTERNALCELL
------------------- Blank : NO discrepancy is found

