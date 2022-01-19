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
request - https://pypi.org/project/requests/
jwt - https://pyjwt.readthedocs.io/en/stable/
flask - https://flask.palletsprojects.com/en/2.0.x/
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
```bash

```
Our tokens saved in database
## License
[MIT](https://choosealicense.com/licenses/mit/)
