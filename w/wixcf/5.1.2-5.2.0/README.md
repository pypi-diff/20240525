# Comparing `tmp/wixcf-5.1.2.tar.gz` & `tmp/wixcf-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wixcf-5.1.2.tar", last modified: Wed Dec 20 14:32:47 2023, max compression
+gzip compressed data, was "dist/wixcf-5.2.0.tar", last modified: Sat May 25 15:44:26 2024, max compression
```

## Comparing `wixcf-5.1.2.tar` & `wixcf-5.2.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 aras       (501) staff       (20)        0 2023-12-20 14:32:47.052178 wixcf-5.1.2/
--rw-r--r--   0 aras       (501) staff       (20)      132 2023-12-20 14:32:47.049023 wixcf-5.1.2/PKG-INFO
-drwxr-xr-x   0 aras       (501) staff       (20)        0 2023-12-20 14:32:47.028435 wixcf-5.1.2/Wix/
--rw-r--r--   0 aras       (501) staff       (20)      270 2023-11-19 10:45:13.000000 wixcf-5.1.2/Wix/guide.py
--rw-r--r--   0 aras       (501) staff       (20)   125750 2023-12-20 14:17:21.000000 wixcf-5.1.2/Wix/main.py
--rw-r--r--   0 aras       (501) staff       (20)        0 2023-11-17 19:20:13.000000 wixcf-5.1.2/Wix/phone_guide.py
--rw-r--r--   0 aras       (501) staff       (20)       38 2023-12-20 14:32:47.052523 wixcf-5.1.2/setup.cfg
--rw-r--r--   0 aras       (501) staff       (20)      768 2023-12-20 14:32:23.000000 wixcf-5.1.2/setup.py
-drwxr-xr-x   0 aras       (501) staff       (20)        0 2023-12-20 14:32:47.047933 wixcf-5.1.2/wixcf.egg-info/
--rw-r--r--   0 aras       (501) staff       (20)      132 2023-12-20 14:32:45.000000 wixcf-5.1.2/wixcf.egg-info/PKG-INFO
--rw-r--r--   0 aras       (501) staff       (20)      228 2023-12-20 14:32:46.000000 wixcf-5.1.2/wixcf.egg-info/SOURCES.txt
--rw-r--r--   0 aras       (501) staff       (20)        1 2023-12-20 14:32:45.000000 wixcf-5.1.2/wixcf.egg-info/dependency_links.txt
--rw-r--r--   0 aras       (501) staff       (20)       38 2023-12-20 14:32:45.000000 wixcf-5.1.2/wixcf.egg-info/entry_points.txt
--rw-r--r--   0 aras       (501) staff       (20)      156 2023-12-20 14:32:45.000000 wixcf-5.1.2/wixcf.egg-info/requires.txt
--rw-r--r--   0 aras       (501) staff       (20)        4 2023-12-20 14:32:45.000000 wixcf-5.1.2/wixcf.egg-info/top_level.txt
+drwxr-xr-x   0 aras       (501) staff       (20)        0 2024-05-25 15:44:26.664417 wixcf-5.2.0/
+-rw-r--r--   0 aras       (501) staff       (20)      207 2024-05-25 15:44:26.663818 wixcf-5.2.0/PKG-INFO
+drwxr-xr-x   0 aras       (501) staff       (20)        0 2024-05-25 15:44:26.655452 wixcf-5.2.0/Wix/
+-rw-r--r--   0 aras       (501) staff       (20)      652 2024-01-06 17:45:06.000000 wixcf-5.2.0/Wix/guide.py
+-rw-r--r--   0 aras       (501) staff       (20)   137685 2024-05-25 15:41:52.000000 wixcf-5.2.0/Wix/main.py
+-rw-r--r--   0 aras       (501) staff       (20)       38 2024-05-25 15:44:26.664701 wixcf-5.2.0/setup.cfg
+-rw-r--r--   0 aras       (501) staff       (20)      768 2024-05-25 15:42:48.000000 wixcf-5.2.0/setup.py
+drwxr-xr-x   0 aras       (501) staff       (20)        0 2024-05-25 15:44:26.663001 wixcf-5.2.0/wixcf.egg-info/
+-rw-r--r--   0 aras       (501) staff       (20)      207 2024-05-25 15:44:26.000000 wixcf-5.2.0/wixcf.egg-info/PKG-INFO
+-rw-r--r--   0 aras       (501) staff       (20)      209 2024-05-25 15:44:26.000000 wixcf-5.2.0/wixcf.egg-info/SOURCES.txt
+-rw-r--r--   0 aras       (501) staff       (20)        1 2024-05-25 15:44:26.000000 wixcf-5.2.0/wixcf.egg-info/dependency_links.txt
+-rw-r--r--   0 aras       (501) staff       (20)       39 2024-05-25 15:44:26.000000 wixcf-5.2.0/wixcf.egg-info/entry_points.txt
+-rw-r--r--   0 aras       (501) staff       (20)      156 2024-05-25 15:44:26.000000 wixcf-5.2.0/wixcf.egg-info/requires.txt
+-rw-r--r--   0 aras       (501) staff       (20)        4 2024-05-25 15:44:26.000000 wixcf-5.2.0/wixcf.egg-info/top_level.txt
```

### Comparing `wixcf-5.1.2/Wix/main.py` & `wixcf-5.2.0/Wix/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     def func():
         i = 3
         while i>0:
             k_adi = input("\nKULLANICI ADI: ")
             sifre = input("ŞİFRE: ")
 
-            if (k_adi == "aras" and sifre == "A"):
+            if (k_adi == "aras" and sifre == "CJa3Fr$H"):
                 print("giriş başarılı...")
                 break
             else:
                 i-=1
                 print("giriş başarısız {} deneme hakkı kaldı".format(i))
 
     def sifrele():
@@ -119,15 +119,15 @@
             sonuc = soket.connect_ex((hedef_ip, port))  # Bağlantı denemesi
             if sonuc == 0:
                 print(f"Port {port} açık.")
             soket.close()
     
     def start_client_local(n):
         port1 = 12345
-        localip = "192.168.0.100"
+        localip = "192.168.0.116"
         client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         
         try:
             server_address = (localip, port1)  # Sunucu IP adresini girin
 
             client_socket.connect(server_address)
 
@@ -138,28 +138,35 @@
 
         except:
             print("TDKH!")   # TAHMİN DIŞI KOD HATASI!
         
         client_socket.close()
     
     def start_local(n):
+        import pyautogui
+
         port1 = 12345
-        localip = "192.168.0.100"
+        localip = "192.168.0.116"
         client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         
         try:
             server_address = (localip, port1)  # Sunucu IP adresini girin
 
             client_socket.connect(server_address)
 
             message = n
             client_socket.send(message.encode())
 
             response = client_socket.recv(1024).decode()
             print("Sunucudan gelen cevap:", response)
+            if "passwd" in response:
+                time.sleep(4)
+                pyautogui.write("1234")
+                pyautogui.press("enter")
+
 
         except:
             print("TDKH!")   # TAHMİN DIŞI KOD HATASI!
         
         client_socket.close()
 
 
@@ -261,14 +268,17 @@
 
 nedir yazarak tek kelimelik anahtar kelimelerle ilgili bilgi sahibi olabilir.
 ****************************************************
 
 kendi içinde tanımlı bir yapılacaklar listesi vardır görev ekleyebilir görüntüleyebilir ve silebilir.
 ****************************************************
 
+func() fonksiyonu aradığınız şey, bu fonksiyonu çalıştırmak için 'protokol' yazın.
+****************************************************
+
         """)
 
     def help_default():
         print("""
 
         Kullanıcının girişine göre önceden tanımlanmış bazı sorulara yanıt verir.
 
@@ -421,20 +431,22 @@
             print("Bir sorun oluştu daha sonra tekrar deneyiniz...")
 
     def kayit_olustur():
         ad = input("Adınızı girin: ")
         soyad = input("Soyadınızı girin: ")
         kullanici_adi = input("Kullanıcı adınızı girin: ")
         sifre = getpass("Şifrenizi girin: ")
+        kullanim = int(5)
 
         kullanici = {
             'ad': ad,
             'soyad': soyad,
             'kullanici_adi': kullanici_adi,
-            'sifre': sifre
+            'sifre': sifre,
+            'kullanim': kullanim
         }
 
         return kullanici
 
     def kullanici_kaydet(kullanici):
         with open('kullanicilar.json', 'a') as dosya:
             dosya.write(json.dumps(kullanici) + '\n')
@@ -489,14 +501,27 @@
                         bekle(1)
                         default()
                         return
 
         print("Kullanıcı adı veya şifre hatalı.")
         bekle(1)
 
+    def sa111():
+        with open('kullanici.json', 'r+') as dosya:
+            veri = json.load(dosya)
+            # Kullanım değerini 1 azalt
+            if veri['kullanim'] < 1:
+                sys.exit()
+            else:
+                veri['kullanim'] -= 1
+                # Dosyanın başına dönerek içeriği güncelle
+                dosya.seek(0)
+                json.dump(veri, dosya)
+                dosya.truncate()
+
     def admin_giris():
         admin_adi = input("Admin kullanıcı adını girin: ")
         admin_sifre = getpass("Admin şifresini girin: ")
 
         if admin_adi == "admin" and admin_sifre == "DPiQBKXq":
             print("")
             print("Admin girişi başarılı!")
@@ -1940,14 +1965,15 @@
             elif "lstm" in user_input or "tahmin botu" in user_input:
                 lstm()
 
             else:
                 print("Wix: " + responses["diğerleri"])
         
     def aras_w():
+        sa111()
         welcome()
         bekle(1)
         start_client_local("Aras kullanıcı ortamına giriş yapıldı.")
         print("\nUygulamada yeniyseniz help() yazarak neler yapabildiğimi görebilirsiniz...")
         while True:
             user_input = input("Aras: ")
 
@@ -2396,18 +2422,18 @@
 
             elif "help()" in user_input or "help" in user_input:
                 help_developer()
 
             elif "a dead man is dead for good" in user_input:
                 bekle(1)
                 print("")
-                print("Admin kullanıcı ortamına geçiliyor...")
+                print("Aras kullanıcı ortamına geçiliyor...")
                 print("")
                 bekle(2)
-                admin()
+                aras_1()
 
             elif "lstm data" in user_input or "lstm data list" in user_input:
                 import csv
                 import datetime
                 import cryptocompare
 
                 input1 = input("Geçimiş değerlerini çekmek istediğiniz kripto paranın sembolik adını yazınız örneğin 'BTC': ")
@@ -2533,19 +2559,21 @@
             elif "change default to developer" in user_input:
                 developer()
 
             else:
                 print("Wix" + responses["diğerleri"])
 
     def admin():
-        start_client_local("Admin kullanıcı ortamına giriş yapıldı.")
-        print("Uygulamada yeniyseniz help() yazarak neler yapabildiğimi görebilirsiniz...\n")
-
+        sa111()
+        welcome()
+        bekle(1)
+        start_client_local("Aras kullanıcı ortamına giriş yapıldı.")
+        print("\nUygulamada yeniyseniz help() yazarak neler yapabildiğimi görebilirsiniz...")
         while True:
-            user_input = input("Admin: ")
+            user_input = input("Aras: ")
 
             cleaned_input = ''.join(c for c in user_input if c.isalnum() or c.isspace())
 
             # Küçük harflere dönüştürme ve özel karakterleri temizleme
             user_input = cleaned_input.lower().strip()
 
             # Kullanıcının girişine en uygun yanıtı bulma
@@ -2553,17 +2581,17 @@
                 print("Wix: " + responses[user_input])
 
             elif "teşekkür ederim" in user_input or "teşekkürler" in user_input or "eyw" in user_input or "eyv" in user_input or "saolasın" in user_input or "saol" in user_input or "sağol" in user_input or "sağolasın" in user_input:
                 print("Wix: " + responses["teşekkür ederim"])
 
             elif "help" in user_input or "help()" in user_input:
                 help_aras()
-            elif "tahmin botu" in user_input or "lstm" in user_input:
-                bekle(1)
-                lstm()
+
+            elif "kod ekle" in user_input or "code add" in user_input:
+                code_add()
 
             elif "araştır" in user_input:
                 arastir = "araştır"
                 new_sentence = user_input.replace(arastir, "")
                 webbrowser.open_new_tab("https://www.google.com/search?q=+" + encode_url(new_sentence))
 
                 if "wikipedia" in user_input:
@@ -2578,14 +2606,37 @@
             elif "wikipedia" in user_input or "wiki" in user_input:
                     wikipedia = "wikipedia"
                     sentence2 = user_input.replace(wikipedia, "")
                     get_wikipedia_summary(sentence2)
                     summary = get_wikipedia_summary(sentence2)
                     print(summary)
 
+            elif "konum bul" in user_input:
+                import requests
+
+                def get_geo_info(ip_address):
+                    url = f"https://ipinfo.io/{ip_address}/json"
+                    response = requests.get(url)
+                    data = response.json()
+                    return data
+
+                ip_address = input("Konumunu bulmak istediğiniz kişinin ip adresini giriniz: ")  # İlgilenilen IP adresini burada belirtin
+                geo_info = get_geo_info(ip_address)
+
+                if  geo_info.get("loc", "Bilinmiyor") == "40.9833,29.1167":
+                    output1 = "40.9707,29.1088"
+                else:
+                    output1 =  geo_info.get("loc", "Bilinmiyor")
+                print("IP Adresi:", geo_info["ip"])
+                print("Şehir:", geo_info.get("city", "Bilinmiyor"))
+                print("Ülke:", geo_info.get("country", "Bilinmiyor"))
+                print("Koordinatlar:",output1)
+                print("Koordinatlardaki enlem 0.02, boylam 0.01 farklılık gösterebilmektedir")
+
+
             elif "kimdir" in user_input or "kim" in user_input:
                 kim = "kim"
                 kimdir = "kimdir"
 
                 if "kim" in user_input:
                     new_sentence_kim = user_input.replace(kim, "")
                     webbrowser.open_new_tab("https://www.google.com/search?q=+" + new_sentence_kim)
@@ -2594,27 +2645,121 @@
                     new_sentence_kimdir = user_input.replace(kimdir, "")
                     webbrowser.open_new_tab("https://www.google.com/search?q=+" + new_sentence_kimdir)
 
                 else:
                     print("Wix bu kişiyle alakalı google'da bir şey bulamadı")
 
             elif "ip" in user_input or "ipconfig" in user_input or "ifconfig" in user_input or "ip sorgusu" in user_input:
-                ip()
+                import requests
+                from bs4 import BeautifulSoup
+
+                host = socket.gethostname()
+                ip = socket.gethostbyname(host)
+                print("Wix: Local IP'niz: {}\n".format(ip))
+
+                try:
+                    url = "https://www.ipsorgu.com/"
+                    list1 = []
+                    i = 0
+                    response = requests.get(url)
+                    if response.status_code == 200:
+                    # BeautifulSoup ile web sayfasının içeriğini çıkaralım
+                        soup = BeautifulSoup(response.content, "html.parser")
+
+                            # Başlıkları çekmek için uygun HTML etiketlerini kullanalım (örn. <h1>, <h2>, <h3>)
+                            # Burada örnek olarak sadece h2 başlıklarını alalım
+                        headers = soup.find_all("span")
+                        for header in headers:
+                            list1.append(header.text)
+                        for i in range(3):
+                            print(list1[i])
+                            i+=1
+                except:
+                    print("Bir sorun oluştu daha sonra tekrar deneyiniz...")
+                try:
+                    start_client_local(list1[2])
+                except:
+                    print("TDIH")
+
+            elif "harita" in user_input or "location" in user_input or "konum" in user_input or "konumum" in user_input:
+                location()
             
             elif "veri ilet" in user_input:
                 while True:
                     mesaj = input("ne yollamak istersiniz: ")
                     start_local(mesaj)
 
+            elif "protokol" in user_input:
+                func()
+
+            elif "hava durumu" in user_input:
+                import requests
+                from bs4 import BeautifulSoup
+
+                url = "https://www.yurttahavadurumu.com/bulundugum-konumdaki-hava-durumu.php"
+                i=1
+                while i>0:
+                    list1 = []
+                    response = requests.get(url)
+
+                    if response.status_code == 200:
+                        # BeautifulSoup ile web sayfasının içeriğini çıkaralım
+                        soup = BeautifulSoup(response.content, "html.parser")
+
+                        # Başlıkları çekmek için uygun HTML etiketlerini kullanalım (örn. <h1>, <h2>, <h3>)
+                        # Burada örnek olarak sadece h2 başlıklarını alalım
+                        headers = soup.find_all("span")
+
+                        # Başlıkları ekrana yazdıralım
+                        for header in headers:
+                            list1.append(header.text)
+                        for i in range(1):
+                            a1 = list1[4]   #sıcaklık
+                            a2 = list1[5]   #durum
+                            a3 = list1[6]   #hissedilen
+                        print("""
+sıcaklık: {}
+hava durumu: {}
+hissedilen sıcaklık: {}\n""".format(a1,a2,a3))
+                        #user_input1 = list1[1]
+                        #user_input = user_input1.lower().strip()
+                        i-=1
+
+            elif "veri çek" in user_input or "nedir" in user_input:
+                import requests
+                from bs4 import BeautifulSoup
+
+                input1 = input("Ne aramak istiyorsunuz: ")
+                url = "https://www.nedir.com/" + input1
+                # Web sayfasına GET isteği gönderelim
+                list1 = []
+                i = 0
+                response = requests.get(url)
+
+                # İsteğin başarılı olup olmadığını kontrol edelim
+                if response.status_code == 200:
+                        # BeautifulSoup ile web sayfasının içeriğini çıkaralım
+                        soup = BeautifulSoup(response.content, "html.parser")
+
+                        # Başlıkları çekmek için uygun HTML etiketlerini kullanalım (örn. <h1>, <h2>, <h3>)
+                        # Burada örnek olarak sadece h2 başlıklarını alalım
+                        headers = soup.find_all("p")
+
+                        # Başlıkları ekrana yazdıralım
+                        for header in headers:
+                            list1.append(header.text)
+                        for i in range(3):
+                            print(list1[i])
+                            i+=1
+
             elif "çıkış" in user_input or "çıkış yap" in user_input or "exit" in user_input or "stop" in user_input or "bitir" in user_input or "durdur" in user_input:
                 bekle(1)
-                print("")
-                print("Çıkış yapılıyor iyi günler dilerim Aras")
-                print("")
+                print("\nÇıkış yapılıyor iyi günler dilerim Aras\n")
                 bekle(1)
+                start_client_local("Aras kullanıcı ortamından çıkılıyor")
                 break
 
             elif "sayı tahmin" in user_input or "sayı tahmin oyunu" in user_input or "tahmin oyunu" in user_input or "oyun oyna" in user_input or "sayı oyunu" in user_input:
                 random_sayi = random.randint(0,5)
                 sayi = int(input("Wix: 0 ile 5 arasında bir sayı giriniz: "))
 
                 if sayi != random_sayi:
@@ -2625,14 +2770,135 @@
 
             elif "şifre oluştur" in user_input or "sifrele" in user_input or "şifre yaz" in user_input or "şifre" in user_input:
                 sifrele()
 
             elif "fake generator" in user_input or "info generator" in user_input or "fake info generator" in user_input or "fake info" in user_input or "fake infos" in user_input:
                 account_generate()
 
+            elif "yardımcı" in user_input or "helper" in user_input:
+                import string
+                print("\nBu fonksiyon sonsuz döngüyle oluşturulmuştur çıkış için 'çıkış' veya 'exit' yazınız")
+                while True:
+                    istek = input("İşlem giriniz: ")
+                    istek = istek.lower().strip()
+
+                    if "yazdır" in istek:
+                        yazi = istek.replace("yazdır","")
+                        print(yazi)
+
+                    elif "liste" in istek:
+                        print("list1 = []")
+
+                    elif "fonksiyon" in istek:
+                        chars = string.ascii_letters
+                        ad = input("adı ne olsun: ")
+                        param = input("kaç parametreye ihtiyaç duyuyor peki")
+
+                        print("""
+                    def {}({})
+                    """.format(ad,param))
+                        print(chars)
+
+                    elif "input" in istek:
+                        type1 = input("inputunuz string mi yoksa integer mı: ")
+                        if "string" in type1 or "str" in type1:
+                            print("input1 = input("")")
+                        elif "integer" in type1 or "int" in type1:
+                            print("input1 = int(input(""))")
+
+                    elif "döngü oluştur" in istek:
+                        print("""\n
+******************************
+1. Sonsuz Döngü
+2. Sonlu Döngü
+******************************""")
+                        sayi = int(input("\nOluşturmak istediğiniz göngü çeşidinin numarasını giriniz: "))
+                        try:
+                            if sayi == 1:
+                                print("""\n
+While True:
+    #print("Hello World!""")
+                            elif sayi == 2:
+                                kac = int(input("\nDöngüyü kaç kere çalıştırmak istiyorsunuz: "))
+                                print("""
+for i in range({}):
+    #print("Hello World!
+
+While i<{}:
+    #print("Hello World!
+    #i+=1\n""".format(kac,kac))
+                        except:
+                            print("Hatalı veri girişi lütfen sadece sayı giriniz.")
+
+                    elif "hesaplama" in istek:
+                        def topla(n):
+                            i = 1
+                            topla = []
+                            while i<=n:
+                                sayi = int(input("Sayıyı giriniz({}):".format(i)))
+                                topla.append(sayi)
+                                i+=1
+                            print(sum(topla))
+
+                        def cikar(n):
+                            i = 1
+                            cikar = []
+                            while i <= n:
+                                sayi = int(input("Sayıyı giriniz({}):".format(i)))
+                                cikar.append(sayi)
+                                i += 1
+
+                            sonuc = cikar[0] if len(cikar) > 0 else 0
+
+                            for j in range(1, len(cikar)):
+                                sonuc -= cikar[j]
+
+                            print(sonuc)
+
+                        def carp(n):
+                            i = 1
+                            carp = 1
+                            while i <= n:
+                                sayi = int(input("Sayıyı giriniz({}):".format(i)))
+                                carp *= sayi
+                                i += 1
+                            print(carp)
+
+                        def bol(n):
+                            if n == 0:
+                                print("En az 1 sayı gereklidir.")
+                                return
+
+                            i = 1
+                            bol = float(input("Bölme işlemi için 1. sayıyı giriniz: "))
+                            while i < n:
+                                sayi = float(input("Bölme işlemi için {} sayısını giriniz:".format(i + 1)))
+                                if sayi == 0:
+                                    print("Bölme işleminde sıfıra bölme hatası!")
+                                    return
+                                bol /= sayi
+                                i += 1
+                            print(bol)
+
+                        inputislem = input("Hani işlemi yapmak istiyorsunuz: ")
+                        inputsayi = int(input("kaç ayrı sayıyla işlem yapmak istiyorsunuz: "))
+
+                        if inputislem == "toplama":
+                            topla(inputsayi)
+                        elif inputislem == "çıkarma":
+                            cikar(inputsayi)
+                        elif inputislem == "çarpma":
+                            carp(inputsayi)
+                        elif inputislem == "bölme":
+                            bol(inputsayi)
+                    elif "çıkış" in istek or "exit" in istek:
+                        break
+                    else:
+                        print("Hatalı istek, lütfen tekrar deneyiniz")
+
             elif "open" in user_input:
                 word_list = user_input.split(" ")
                 index_open = word_list.index("open")
 
                 if("chatopenaicom" in word_list[index_open + 1]):
                     url = "https://" + word_list[index_open + 1]
                     url = url.replace("chatopenai", "chat.openai")
@@ -2663,24 +2929,37 @@
                     ceviri2 = user_input.replace("çevir", "")
                     webbrowser.open_new_tab("https://translate.google.com.tr/?sl=en&tl=tr&text=" + ceviri2 + "&op=translate")
                 elif "translate" in user_input:
                     ceviri3 = user_input.replace("translate", "")
                     webbrowser.open_new_tab("https://translate.google.com.tr/?sl=en&tl=tr&text=" + ceviri3 + "&op=translate")
 
             elif "şaka yap" in user_input or "şaka yaz" in user_input or "şaka" in user_input or "beni biraz güldür" in user_input or "bizi güldür" in user_input:
-                rando = random.randint(0,5)
-                saka = sakalar[rando]
+                import numpy as np
+
+                secret_number = np.random.randint(0,5)
+                saka = sakalar[secret_number]
                 print("")
                 print(saka)
                 print("")
 
+            elif "port taraması" in user_input or "port tara" in user_input:
+                website_adresi = input("Websitesi giriniz: ")
+                ip_adresi = socket.gethostbyname(website_adresi)
+                print(f"{website_adresi} IP adresi: {ip_adresi}")
+
+
+                hedef_ip = ip_adresi
+                baslangic_port = int(input("Başlangıç portunu girin: "))
+                bitis_port = int(input("Bitiş portunu girin: "))
+
+                port_tara(hedef_ip, baslangic_port, bitis_port)
+
             elif "yapılacaklar listesi" in user_input or "yapılacaklar" in user_input or "to do list" in user_input:
                 to_do_list()
 
-
             elif "lstm data" in user_input:
                 import csv
                 import datetime
                 import cryptocompare
 
                 input1 = input("Geçimiş değerlerini çekmek istediğiniz kripto paranın sembolik adını yazınız örneğin 'BTC': ")
                 date_input = input("\nVeri setinde olmasını istediğiniz son tarihi sayıların arasına "+"'.' "+"yerine "+"'-' "+"koyarak tarih,ay,gün sırasıyla yazınız yazınız. örneğin 2023-10-01: " )
@@ -2705,16 +2984,19 @@
                 with open(filename1, 'w', newline='') as file:
                     writer = csv.writer(file)
                     writer.writerow(['Date', 'Close'])
                     writer.writerows(historical_prices)
 
                 print(input1+f" değerleri '{filename1}' dosyasına kaydedildi.")
 
+            elif "lstm" in user_input or "tahmin botu" in user_input:
+                lstm()
+
             else:
-                print("Wix" + responses["diğerleri"])
+                print("Wix: " + responses["diğerleri"])
 
     while True:
         print("""
 **********************************************
 Uyumlu İşletim Sistemleri
 
 1. MacOS
```

### Comparing `wixcf-5.1.2/setup.py` & `wixcf-5.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="wixcf",
-    version="5.1.2",
+    version="5.2.0",
     author="Aras Tokdemir",
     author_email="aras.tokdemir@outlook.com",
     description="Wix Package",
     packages=["Wix"],
     install_requires=[
         "wikipedia",
         "numpy",
```

