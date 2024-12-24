# Домашнее задание к занятию 10 «Jenkins»

## Подготовка к выполнению

1. Создать два VM: для jenkins-master и jenkins-agent.
2. Установить Jenkins при помощи playbook.
3. Запустить и проверить работоспособность.
4. Сделать первоначальную настройку.

## Основная часть

1. Сделать Freestyle Job, который будет запускать `molecule test` из любого вашего репозитория с ролью.
2. Сделать Declarative Pipeline Job, который будет запускать `molecule test` из любого вашего репозитория с ролью.
3. Перенести Declarative Pipeline в репозиторий в файл `Jenkinsfile`.
4. Создать Multibranch Pipeline на запуск `Jenkinsfile` из репозитория.
5. Создать Scripted Pipeline, наполнить его скриптом из [pipeline](./pipeline).
6. Внести необходимые изменения, чтобы Pipeline запускал `ansible-playbook` без флагов `--check --diff`, если не установлен параметр при запуске джобы (prod_run = True). По умолчанию параметр имеет значение False и запускает прогон с флагами `--check --diff`.
7. Проверить работоспособность, исправить ошибки, исправленный Pipeline вложить в репозиторий в файл `ScriptedJenkinsfile`.
8. Отправить ссылку на репозиторий с ролью и Declarative Pipeline и Scripted Pipeline.
9. Сопроводите процесс настройки скриншотами для каждого пункта задания!!

## Результат

1.  Сделать Freestyle Job, который будет запускать `molecule test` из любого вашего репозитория с ролью.
   ![Freestyle Job](./images/1.png)
2.  Сделать Declarative Pipeline Job, который будет запускать `molecule test` из любого вашего репозитория с ролью.
   ![Freestyle Job](./images/2.png)  
   ![Freestyle Job](./images/2-2.png)  
3. Перенести Declarative Pipeline в репозиторий в файл `Jenkinsfile`.
   [Jenkinsfile](https://github.com/barmaq/ansible-05-testing/blob/main/Jenkinsfile)
4. Создать Multibranch Pipeline на запуск `Jenkinsfile` из репозитория.  
   ![Freestyle Job](./images/4.png)  
5. Создать Scripted Pipeline, наполнить его скриптом из [pipeline](./pipeline).  
   ![Freestyle Job](./images/5.png)  
6. Внести необходимые изменения, чтобы Pipeline запускал `ansible-playbook` без флагов `--check --diff`, если не установлен параметр при запуске джобы (prod_run = True). По умолчанию параметр имеет значение False и запускает прогон с флагами `--check --diff`.
   ![Freestyle Job](./images/6.png)  
7. Проверить работоспособность, исправить ошибки, исправленный Pipeline вложить в репозиторий в файл `ScriptedJenkinsfile`.
   првоерено
9. Отправить ссылку на репозиторий с ролью и Declarative Pipeline и Scripted Pipeline.
   [Freestyle Job]([./images/6.png](https://github.com/barmaq/ansible-05-testing)) 
10. Сопроводите процесс настройки скриншотами для каждого пункта задания!!
