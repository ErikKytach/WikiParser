import requests
from bs4 import BeautifulSoup
try:
    url = input('Введіть сайт -> ')
    response = requests.get(url)
    if response.status_code == 200:
        content = requests.get(url).text
        soup = BeautifulSoup(content, 'html.parser')
        text = soup.select('p')

    
        for items in text:
            print(items.text)

    else:
        print(False)
except NameError:
    print('Ой, помилка! Такого сайту не існує! Перевірте правильність написання посилання!')
