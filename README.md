## Django
Django is a powerful Web Framework for Python !

1. cd 到資料夾後，在終端機輸入指令，會自動創建模板
  ```django-admin startproject <file_name>```
2. 終端機輸入 (創建連線網址)
  `python manage.py runserver`


## Terminal
- django-admin startproject <file_name> : it will automatically create some templated file for you.
- python manage.py migrate : 可以在不影響現有數據的前提下，重建表結構。
- python manage.py makemigrations main : 用於創建與應用程式中的模型更改相關的數據庫遷移（migrations）
- python manage.py migrate : apply the change
- python manage.py shell : 操作程式 ( ex. 輸入資料... )

### 設定端口
> python manage.py runserver 8080

### SQLite3 DataBase ( terminal 操作 )
- > from main.models import Item, ToDoList
- > t = ToDoList(name='Jack\'s list')
- > t.save()
- > ToDoList.objects.all()
- > t.item_set.all()
- > t.item_set.create(text='go home', complete=False)
- > t.filter(name__startswith='hello')

### Admin dashboard
> python manage.py createsuperuser

-----------------------------------

### Database Models and ORM
提供了一個被稱為 ORM（object relational mapping）的東西，我們可以使用 Python 代碼來創建不同的資料庫模型，我們創建的任何模型都會自動在某種結構化的資料庫架構中生成，比如 SQLite3。

當開始創建這些模型時，會看到將生成一個名為「migration」的東西，這個遷移實際上是自動化的代碼，它將會在類似 SQL、MongoDB 或者我們使用的任何資料庫後端引擎中創建對應的模型。

### Django Migration
是 Django 框架中的一個工具。允許開發者使用 Python 代碼來定義資料庫模型、進行演進，同時保持資料的完整性，而無需手動處理複雜的資料庫遷移操作。

### Django Admin Panel
是 Django 提供的一個特殊工具，允許我們管理使用者和不同的資料庫模型，非常實用。

----------------------

refer : 
- https://www.youtube.com/watch?v=nGIg40xs9e4
- https://pastebin.com/AMzZVL12  ( Django Base Template )
- https://www.youtube.com/watch?v=sm1mokevMWk
