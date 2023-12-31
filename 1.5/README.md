### Домашнее задание к занятию «Сетевое взаимодействие в K8S. Часть 2»

## Цель задания

В тестовой среде Kubernetes необходимо обеспечить доступ к двум приложениям снаружи кластера по разным путям.

## Задание 1. Создать Deployment приложений backend и frontend

1. Создать Deployment приложения frontend из образа nginx с количеством реплик 3 шт.

![Скрин 1](./images/1.png)

2. Создать Deployment приложения backend из образа multitool.

![Скрин 2](./images/2.png)

3. Добавить Service, которые обеспечат доступ к обоим приложениям внутри кластера.

![Скрин 3](./images/3.png)

4. Продемонстрировать, что приложения видят друг друга с помощью Service.

![Скрин 4](./images/4.png)

![Скрин 5](./images/5.png)

5. Предоставить манифесты Deployment и Service в решении, а также скриншоты или вывод команды п.4.

[yaml манифест первый](https://github.com/george25031996/kubernetes-netology/blob/main/1.5/task1.yml)

## Задание 2. Создать Ingress и обеспечить доступ к приложениям снаружи кластера

1. Включить Ingress-controller в MicroK8S.

![Скрин 6](./images/6.png)

2. Создать Ingress, обеспечивающий доступ снаружи по IP-адресу кластера MicroK8S так, чтобы при запросе только по адресу открывался frontend а при добавлении /api - backend.

![Скрин 7](./images/7.png)

3. Продемонстрировать доступ с помощью браузера или curl с локального компьютера

![Скрин 8](./images/8.png)

4. Предоставить манифесты и скриншоты или вывод команды п.2.

[yaml манифест второй](https://github.com/george25031996/kubernetes-netology/blob/main/1.5/task2.yml)
