#
# Name:    run_get_bls_data.py
# Date:    September 14, 2022
# Author:  Sayak Chanda
#
# Description:
#
# Use the c_bls_data class to obtain series of data
# from the US Bureau of Labor Statistics

from c_bls_data import c_bls_data

#
# See the code in c_bls_data.py for descriptions of the class's input parameters. 

#
# Create and instance of c_bls_data to retrieve cpi data for 1) all items and 2) regular gasoline from the years 2003 through 2022.

# Requested BLS data series IDs and titles:
#
# CUSR0000SAO - All items in U.S. city average, all urban consumers, seasonally adjusted
# CUSR0000SETB01 - Gasoline (all types) in U.S. city average, all urban consumers, seasonally adjusted
# CUR0000SAF1 - Food in U.S. city average, all urban consumers, seasonally adjusted
# CUSR0000SETA02 - Used cars and trucks in U.S. city average, all urban consumers, seasonally adjusted
#

c_bls_data('your_registration_key_here', 'c:/bls_data/inflation.csv', ['CUSR0000SA0', 'CUSR0000SETB01', 'CUSR0000SAF1', 'CUSR0000SETA02'], 2003, 2022)
