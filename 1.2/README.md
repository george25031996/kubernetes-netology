
### Домашнее задание к занятию «Базовые объекты K8S»

## Задание 1. Создать Pod с именем hello-world

1. Создать манифест (yaml-конфигурацию) Pod.

![Скрин 1](./images/1.png)

2. Использовать image - gcr.io/kubernetes-e2e-test-images/echoserver:2.2.

Я использовал image nginx, так как с данным image не происходил проброс портов

3. Подключиться локально к Pod с помощью kubectl port-forward и вывести значение (curl или в браузере).

![Скрин 2](./images/2.png)

![Скрин 3](./images/3.png)


## Задание 2. Создать Service и подключить его к Pod

1. Создать Pod с именем netology-web

![Скрин 4](./images/7.png)

2. Использовать image — gcr.io/kubernetes-e2e-test-images/echoserver:2.2

Я использовал опять image nginx, так как с данным image не происходил проброс портов

3. Создать Service с именем netology-svc и подключить к netology-web.

![Скрин 5](./images/8.png)

![Скрин 6](./images/4.png)

Я использовал Service netology-svc2, так как netology-svc у меня не заработал.

4. Подключиться локально к Service с помощью kubectl port-forward и вывести значение (curl или в браузере).

![Скрин 7](./images/5.png)

![Скрин 8](./images/6.png)

## Правила приёма работы

1. Домашняя работа оформляется в своем Git-репозитории в файле README.md. Выполненное домашнее задание пришлите ссылкой на .md-файл в вашем репозитории.

2. Файл README.md должен содержать скриншоты вывода команд kubectl get pods, а также скриншот результата подключения. 

![Скрин 9](./images/9.png)

3. Репозиторий должен содержать файлы манифестов и ссылки на них в файле README.md.

[yaml манифест](https://github.com/george25031996/kubernetes-netology/blob/main/1.2/pod%2Bservice.yaml)
