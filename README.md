# Домашнее задание к занятию 10 «Jenkins»



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
   проверено  
9. Отправить ссылку на репозиторий с ролью и Declarative Pipeline и Scripted Pipeline.  
   [Declarative pipeline](./declarative)   
   [Scripted pipeline](./scripted)    
   [Repository](https://github.com/barmaq/ansible-05-testing)   

