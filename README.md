# Интеграция L7-балансировщика с Yandex Cloud CDN и Yandex Object Storage

В качестве бэкенда L7-балансировщика Yandex Application Load Balancer используется бакет [Yandex Object Storage](https://yandex.cloud/ru/docs/storage/). Запросы пользователей передаются балансировщику через сеть распространения контента [Yandex Cloud CDN](https://yandex.cloud/ru/docs/cdn/), чтобы сократить время доставки контента.

Для реализации решения потребуется ваш собственный домен. Для выпуска сертификата потребуется подтвердить права владения этим доменом.

Настройка описана в [практическом руководстве](https://yandex.cloud/ru/docs/application-load-balancer/tutorials/cdn-storage-integration). В репозитории хранятся конфигурационные файлы для развертывания инфраструктуры с помощью Terraform:

`yc-cdn-storage-integration-config.tf` — манифест Terraform для создания облачной инфраструктуры.
`yc-cdn-storage-integration.auto.tfvars` — файл c пользовательскими данными.
