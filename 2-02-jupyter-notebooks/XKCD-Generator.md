## Pip

```bash
pip install requests
pip install beautifulsoup
```


```python
import requests
```


```python
import bs4
```


```python
requests.get("https://xkcd.com")
```


```python
response = requests.get("https://xkcd.com")
```


```python
response.content
```


```python
import bs4
import requests
import random

random.seed(5)

comic_number = random.randint(1, 2034)

response = requests.get(f"https://xkcd.com/{comic_number}")

body = response.content.decode("utf-8")

soup = bs4.BeautifulSoup(body, "lxml")

url_to_comic = soup.findAll("img")[1]["src"].replace("//", "https://")

from IPython.display import display

response = requests.get(url_to_comic)

from PIL import Image
from io import BytesIO

r = requests.get(url_to_comic)

im = Image.open(BytesIO(r.content))

im
```

![](./XKCD-Generator_files/XKCD-Generator_2_0.png)

