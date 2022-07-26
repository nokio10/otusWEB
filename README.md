# otusWEB

## Задание 

Варианты стенда:

nginx + php-fpm (laravel/wordpress) + python (flask/django) + js(react/angular);
nginx + java (tomcat/jetty/netty) + go + ruby;
можно свои комбинации. Реализации на выбор:
на хостовой системе через конфиги в /etc;
деплой через docker-compose. Для усложнения можно попросить проекты у коллег с курсов по разработке К сдаче принимается:
vagrant стэнд с проброшенными на локалхост портами
каждый порт на свой сайт
через нжинкс Формат сдачи ДЗ - vagrant + ansible

## Решение

Перед развертыванием VM необходимо заменить ```scr``` в файле prov.yml на акутуальный путь до директирии проекта на локальной машине. 

```
  - name: Copy project
    copy:
      src: /root/otusWEB
      dest: /home/vagrant
```

Проверяю работу после развертывания командой ```vagrant up```

![image](https://user-images.githubusercontent.com/98832702/180997308-3994de80-25c9-475f-9883-e4809a542a91.png)

![image](https://user-images.githubusercontent.com/98832702/180997340-676cc2f4-ebed-43ec-8d7a-863ec337f409.png)

![image](https://user-images.githubusercontent.com/98832702/181000656-44fd7926-ce09-4e5a-b7a0-722e7d7737f0.png)

