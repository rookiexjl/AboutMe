# AboutMe
一个非常简单的博客
# 运行博客，访问地址为http://127.0.0.1:8000
python manage.py runserver 0.0.0.0:8000
# 修改后台管理密码
# python manage.py shell
In [1]: from django.contrib.auth.models import User

In [2]: user = User.objects.get(username='admin')

In [3]: user.set_password('admin')

In [4]: user.save()

In [5]: quit
