

```python
import bs4
import requests
import random
```


```python
random.seed(0)
```


```python
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




![png](XKCD-Generator_files/XKCD-Generator_2_0.png)


