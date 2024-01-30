# liquibase-get
Чтобы сгенерить чейнджесеты нужно описать подключение в liquibase.properties
Далее выбрать вкладку maven -> Plugins -> liquibase -> liquibase:GenerateChangeLog
В ресурсах появится db/changelog со всем необходимым для миграции. Необходимо переименовать в db.changelog-master.xml
И в пути к сетам по заполнению убрать путь от ресурсов, а вставить db/changelog/data/customs_status.csv вместо src/main/resources/db/changelog/data/customs_status.csv
И запустить приложение. Все накатится в новую БД