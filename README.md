# analise-redes

Para rodar é necessário instalar o Jupyter Notebook atráves do Anaconda
```
https://www.anaconda.com/products/distribution
```

Instalar o PyMongo no Anaconda Prompt ou Anaconda Prompt PowerShell
```
Windows: python -m pip install pymongo
```

Criar uma conta no MongoDB e criar uma Database
```
https://www.mongodb.com/atlas/database
```

Conexão do sua Database do MongoDB com Python
```python
import pymongo
from pymongo import MongoClient

cluster = MongoClient("mongodb+srv://<user>:<password>@<cluster>.mongodb.net/<database>?retryWrites=true&w=majority")

db = cluster["<database>"]

collection_transfers = db["<collection>"]
```
