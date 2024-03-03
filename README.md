# Bizcard-
Bizcard is to automate the process of extracting key details from business card images, such as the name, designation, company, contact information, and other relevant data. By leveraging the power of OCR (Optical Character Recognition) provided by EasyOCR, Bizcard is able to extract text from the images.


Introduction
•	In today's fast-paced business environment, efficiently managing and organizing contact information is crucial for successful networking and communication. With the advent of digital tools and technologies, manual entry of business card details into a database can be time-consuming and prone to errors. To overcome these challenges, developers can leverage the power of optical character recognition (OCR) and databases to automate the process of extracting relevant information from business cards and storing it for easy access.
•	One powerful OCR library that facilitates the extraction of text from images is EasyOCR. EasyOCR is an open-source Python library that utilizes deep learning models to accurately recognize and extract text from various languages. By integrating EasyOCR with a MySQL database, developers can streamline the process of capturing business card data and storing it in a structured and organized manner.



Developer Guide
1. Tools Install
•	Virtual code.
•	Python 3.11.0 or higher.
•	MySQL.
2. Requirement Libraries to Install
•	pip install pandas easyocr numpy Pillow opencv-python-headless os re sqlalchemy mysql-connector-python streamlit
3.Import Libraries
import streamlit as st
from streamlit_option_menu import option_menu
import easyocr
from PIL import Image
import pandas as pd
import numpy as np
import re
import mysql.connector
import io
Data frame libraries
•	import pandas as pd
Database Library
•	import sqlalchemy
•	import mysql.connector
•	from sqlalchemy import create_engine, inspect
Dashboard library
•	import streamlit as st
4. E T L Process
a) Extract data
•	Extract relevant information from business cards by using the easyOCR library
b) Process and Transform the data
•	After the extraction process, process the extracted data based on Company name, Card Holder, Designation, Mobile Number, Email, Website, Area, City, State, and Pincode is converted into a data frame.
c) Load data
•	After the transformation process, the data is stored in the MySQL database.
