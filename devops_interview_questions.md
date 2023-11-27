##### DEVOPS INTERVIEW QUESTIONS

### Методологии, DevOps практики, общие вопросы

Agile vs Devops  
Монолит vs Микросервисы  
Continuous Integration  
Continuous Delivery  
Continuous Deployment  
Continuous Testing  
Continuous Monitoring  
GitOps  

---

### Clouds

Elastic IP addresses  
Public ip vs elastic ip  
AWS Elastic Beanstalk  
Policy evaluation logic  
Allow and deny in IAGS  

---

### CI\CD

Опишите условный пайплайн  
Upstream and downstream jobs in Jenkins  

---

### Linux

Load average  
Inodes  
Swap into sysctl – vm.swappiness=<Int from 0 to 100>  
Lsof <path_to_file> or lsof +D <path_to_directory>  
Nohup  
Удалили файл логов nginx, нужно восстановить его содержимое, процесс еще запущен, машина не перезагружалась  
Сигналы  
    - что такое  
    - какие бывают  
    - sync  
    - fork  
двойные кавычки vs одинарные кавыски vs обратные кавычки  
`#!`  
shutdown -h  
jar VS war  
chmod -x /bin/chmod  
Что такое systemd  
Как появляются процессы  
Состояния процессов  
Зомби процессы и сироты  
Как появляются зомби процессы  
apt:  
    - найти пакет  
    - найти пакет в составе package  
Перенаправление ввода/вывода  

---

### GIT

Fetch vs Pull  

---

### Networks(TCP/IP)

Что такое IP адрес  
ЧТо такое маска подсети, объясни как можно проще, чтобы HR поняла  
Маска /25  
OCI model vs TCP\IP model  
TCP vs UDP  
TCP трехстороннее рукопожатие  
Как размещается несколько доменов на одном IP(Header Host)  
TSL/SSL:  
    - SERVER NAME EXTANTION  
    - certificate HTTPS\TLS - where is files  
HTTP:  
    - v1 vs v2  
    - Коды ошибок  
    - Разница между кодами 301, 302, 307, 308  
MTU
Jumbo frames
Что происходит когда набираешь curl google.com(Что происходит после ввода адреса ya.ru в браузер?)
Proxy vs VPN
Что такое сеть доставки контента (CDN)
NAT vs PAT
traceroute vs mtr
iptables:  
    - список цепочек  
    - DROP vs REJECT  

---

### Nginx

nginx vs apache  
nginx server_name _  
Проверка конфига  

---

### Ansible

Какую модель использует(pull или push)  
Плюсы/Минусы  
На каком языке написан  
Приоритет переменных  
Структура роли, за что отвечает каждая папка  
ansible.builtin.lineinfile  
ansible.builtin.shell  
Хендлеры  
Модули  

---

### Monitoring

Золотые сигналы  

---

### Kubernetes

Для чего нужна оркестрация  
Схема взаимодействия компонентов кластера  
Control plane компоненты  
Worker node компоненты  
Что такое kubelet  
Что будет если kubelet остановить  
Что происходит когда выполняешь kubectl apply -f pod.yml  
Что происходит когда выполняешь kubectl get nodes  
Как работает scheduler  
Qos и Qos классы  
NodeAfinity & AntiAfinity vs PodAfinity  
Taints and Tolerations, NoSchedule, PreferNoSchedule и NoExecute  
Pods - Restart Policy  
Init Containers  
Liveness, Readiness and Startup Probes  
Managing Resources for Containers - ???  
Vertical Pod autoscaling  
Horizontal Pod Autoscaler  
DeamonSet  
StatefulSet  
Job  
CronJob  
RBAC  
Services:  
    - ClusterIP  
    - Nodeport  
    - Loadbalancer  
    - ExternalName  
kube-proxy:  
    - iptables  
    - ipvs  
Политика requests=limits  
Стратегии деплоя  
Переопределение CMD и ENTRYPOINT  
CRI - какие бывают  
CNI:  
    - какие бывают  
    - calico  
    - flannel  
    - weavenet  

---

### Docker

Для чего нужна контейнеризация  
Контейнеры vs Виртуальные машины  
Docker run hello-world – Permission denied(Пользователь в группу докер)  
Сети в докере – какая сетка будет при выполнении команды “Docker run nginx”; какие по умолчанию  
Кеш в докере при сборки образа  
Что такое Registry, какие бывают, какие используете  
multistage build  
Стороннее ядро windows, возможно ли запустить на Windows например linux  

---

### BASH

Debugging a Bash Script  
BASH_VERSINFO  

---

### DB

Как вывести список активных соединений на PostgreSQL?  

---

### Python

Передавать аргументы в командной строке  
Структуры данных  
List vs tuple  
Аннотации  
Очереди - deque  
Менеджер контекста  
Работа с  JSON  
Механизм интернирования(256, 257)  

### Terraform

Импорт существующих ресурсов  
Можно ли править вручную tfstate  
Cloud-Init  
	
### Kafka

Для чего нужны брокеры сообщений  

