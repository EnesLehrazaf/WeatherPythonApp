# WeatherPythonApp
Python'da Hava Durumu uygulaması
Bu kod, haber başlıkları almak için bir arayüz sağlayan bir PyQt6 uygulamasıdır. Ayrıca, alınan başlıkları e-posta yoluyla belirtilen adrese gönderir. İşte kodun ana bölümlerinin açıklamaları:

import json: JSON verilerini işlemek için kullanılan standart Python kütüphanesi.
import smtplib: E-posta göndermek için kullanılan SMTP protokolünü uygulayan bir kütüphane.
from email.mime.multipart import MIMEMultipart ve from email.mime.text import MIMEText: E-posta mesajlarını oluşturmak için gerekli olan sınıfları içeren kütüphaneler.
import requests: HTTP istekleri yapmak için kullanılan bir kütüphane.
import sys: Sistemle ilgili işlemleri yapmak için kullanılan bir kütüphane.
from PyQt6.QtWidgets import QApplication, QMainWindow, QLabel, QVBoxLayout, QWidget, QLineEdit, QPushButton, QMessageBox, QListWidget, QListWidgetItem: PyQt6 ile GUI uygulamaları oluşturmak için kullanılan bir dizi sınıf ve fonksiyon.
Kod, MainWindow adlı bir sınıf içerir. Bu sınıf, bir ana pencere oluşturur ve haber başlıklarını almak, e-posta göndermek ve kullanıcı arayüzünü yönetmek için gereken işlevleri sağlar. Ana işlev show_news işlevidir, bu işlev kullanıcının girdiği anahtar kelimeye göre haber başlıklarını alır, bunları ekranda gösterir ve bir e-posta gönderir. Ayrıca, eğer başlıklar alınabilirse kullanıcıya bir bilgi mesajı gösterir, alınamazsa bir hata mesajı gösterir.
