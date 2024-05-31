
1. Открыл архив из Moodle

2. Поменял версию Python yна 3.12.3

3. Заменил PNG на JPEG 

4. Создал виртуальное окружение командой
```
py -m venv venv 
```

Далее я активировал виртуальное окружение командой 
```
.\.venv\Scripts\Activate.ps1
```

5. Запустил сервер на порте 5000 

6. Создал Docker образ 
![[Pasted image 20240531175755.png]]

7. Собрал Docker образ ![[Pasted image 20240531175921.png]]
```
docker build . -t cr.yandex/crp9o8f*******gtc7/flask-application:v.0.0.1
```

8. Запушил этот образ
```
docker push cr.yandex/crp9o8fu********tc7/flask-application:v.0.0.1
```

![[Pasted image 20240531180417.png]]
9. Протестировал работу веб приложения 
![[Pasted image 20240531180521.png]]
![[Pasted image 20240531180511.png]]

![[Pasted image 20240531180846.png]]

Создаем Serverless Containers
![[Pasted image 20240531181144.png]]

Выбрали url образа и создали сервисный аккаунт 
![[Pasted image 20240531181521.png]]

![[Pasted image 20240531181528.png]]

Создаем контейнер 
![[Pasted image 20240531181739.png]]
![[Pasted image 20240531181745.png]]

Работающее приложение из контейнера 
![[Pasted image 20240531181900.png]]

