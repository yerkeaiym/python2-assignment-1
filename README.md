# python2-assignment-1
## Title:
Assignment_1 login Todo app
## Installation

PyPI
```bash
pip install django
pip install psycopg2
pip install jwt
```
or from source
```bash
django - https://docs.djangoproject.com/en/4.0/
psycopg2 - https://www.psycopg.org/docs/
```
## Usage
```bash
urlpatterns = [
    path('login/', CustomLoginView.as_view(), name='login'),
    path('logout/', LogoutView.as_view(next_page='login'), name='logout'),
    path('register/', RegisterPage.as_view(), name='register'),

    path('', TaskList.as_view(), name='tasks'),
    path('task/<int:pk>/', TaskDetail.as_view(), name='task'),
    path('task-create/', TaskCreate.as_view(), name='task-create'),
    path('task-update/<int:pk>/', TaskUpdate.as_view(), name='task-update'),
    path('task-delete/<int:pk>/', DeleteView.as_view(), name='task-delete'),
    path('task-reorder/', TaskReorder.as_view(), name='task-reorder'),
]
```
## Examples
Outputs will be like these:
![image](https://user-images.githubusercontent.com/77783049/150147873-1af45bef-0679-4930-8546-1d03aa7c5ac2.png)
![image](https://user-images.githubusercontent.com/77783049/150147936-c4dbaafe-9561-4051-bd0d-38f3e48dbeaa.png)

```bash

```
Our tokens saved in database
## License
[MIT](https://choosealicense.com/licenses/mit/)
