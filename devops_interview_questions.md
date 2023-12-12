##### DEVOPS INTERVIEW QUESTIONS

### Методологии, DevOps практики, общие вопросы

Agile vs Devops  
Monolith vs Microservices  
Continuous Integration  
Continuous Delivery  
Continuous Deployment  
Continuous Testing  
Continuous Monitoring  
GitOps  

---

### Clouds

## AWS

Elastic IP addresses  
Public ip vs Elastic ip  
AWS Elastic Beanstalk  
Policy evaluation logic  
Allow and deny in IAGS  
S3 versioning
---

### CI\CD

Опишите условный пайплайн 

## Jenkins
 
Upstream and downstream jobs in Jenkins  
Declarative vs imperative  
Multibranch  
Replay vs rebuild  
Метод использования credentials в Jenkins  

---

### Linux

Load average  
Inodes  
Swap into sysctl – vm.swappiness=<Int from 0 to 100>  
Lsof <path_to_file> or lsof +D <path_to_directory>  
Nohup  
Удалили файл логов nginx, нужно восстановить его содержимое, процесс еще запущен, машина не перезагружалась  
Сигналы:  
    - что такое  
    - какие бывают  
    - SIGHUP
    - SIGKILL
    - SIGTERM
Межпроцессное взаимодействие  
Системный вызов fork  
Двойные кавычки vs одинарные кавычки vs машинописный обратный апостроф  
`#!`  
`$?`  
`$1`  
`|`  
`||`  
`&`  
`&&`  
`$!`  
`$@`  
`$$`  
source script.sh VS ./script.sh  
Машинописный обратный апостроф VS $() - $(docker ps -a) VS `docker ps -a`  
Определение переменной в bash с командой export и без нее - export VAR1=abc VS VAR2=abc  
shutdown -h  
jar VS war  
chmod -x /bin/chmod  
Какой первый процесс в Linux  
Что такое systemd  
Отличия initd от systemd  
Как появляются процессы  
Состояния процессов  
Зомби процессы и сироты  
Как появляются зомби процессы  
apt:  
    - найти пакет  
    - найти пакет в составе package  
Перенаправление ввода/вывода  
Как с помощью scp произвести копирование файла  
Что покажет команда ulimit -a  
Как посмотреть все открытые порты на сервере, удаленно, локально  
Как посмотреть размер каталога  
Как посмотреть свободное и занятое место на дисках  
Как посмотреть все открытые порты на сервере локально и удаленно  
Приходилось ли настраивать Linux для высоконагруженных сервисов/систем, что делал  
С какими дистрибутивами работал  
Приходилось ли собирать RPM и/или DEB пакеты  
Какой файл в системе содержит информацию из dmesg  
Hardlink VS symlink  
Какие утилиты используешь для траблшутинга приложений(особенно когда они не отвечают)  
BASH:  
    - Debugging a Bash Script  
    - BASH_VERSINFO  
    - declare -A FOO
    - set -x  
    - set -e  
    - cкобки, двойные, квадратные и двойные квадратные скобки
Для чего нужны директории:  
    - dev  
    - proc  

---

### GIT

Fetch vs Pull  
Как с помощью команды создать новую ветку Git и в нее переключиться  

---

### Networks(TCP/IP)

Что такое IP адрес  
ЧТо такое маска подсети, объясни как можно проще, чтобы HR поняла  
Маска /25  
ARP  
MAC address  
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
По какому порту работает команда ping  
По какому протоколу работает команда ping  

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
hostvars  
group_vars  

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
Как с помощью программы kubectl посмотреть загрузку одной из нод в кластере  
Как работает scheduler  
Qos:
    - Guaranteed  
    - Burstable  
    - BestEffort    
Политика requests=limits  
NodeAfinity & AntiAfinity vs PodAfinity  
Requests and Limits
Priority class and preemption
Taints and Tolerations, NoSchedule, PreferNoSchedule и NoExecute  
Pods - Restart Policy  
Pods lifecycle  
Pod - /etc/resolv.conf ndots:5  
Init Containers  
Liveness, Readiness and Startup Probes  
Managing Resources for Containers - ???  
Vertical Pod autoscaling  
Horizontal Pod Autoscaler  
DeamonSet  
StatefulSet  
Job  
CronJob  
Что такое RBAC? Приходилось ли работать с RBAC? Если да, то что приходилось делать?  
Services:  
    - ClusterIP  
    - Nodeport  
    - Loadbalancer  
    - ExternalName  
    - Headless service  
Как сервис понимает куда направлять траффик если за ним 3 пода  
Как трафик от клиента попадает в pod  
Есть ли внутри k8s средства для управления сетевым трафиком  
kube-proxy:  
    - iptables  
    - ipvs    
Стратегии деплоя:  
    - recreate
    - rolling  
    - blue/green  
    - canary  
    - dark(A/B)  
Переопределение CMD и ENTRYPOINT  
CRI - какие бывают  
CNI:  
    - какие бывают  
    - calico  
    - flannel  
    - weavenet  
Как с помощью программы kubectl посмотреть загрузку одной из нод в кластере  
Admission Controllers  
CPU Throttling  
OOMkilled  
Перенос подов с работающей ноды - drain  
OPA Gatekeeper  
kyverno  


---

### Docker

Для чего нужна контейнеризация  
Контейнеры vs Виртуальные машины  
Образ VS Контейнер  
Запустили контейнер, в нем создали файл, остановили контейнер, файл останется?  
Docker run hello-world – Permission denied(Пользователь в группу докер)  
Сети в докере – какая сетка будет при выполнении команды “Docker run nginx”; какие по умолчанию  
Кеш в докере при сборки образа  
Что такое Registry, какие бывают, какие используете  
multistage build  
Стороннее ядро windows, возможно ли запустить на Windows например linux  
Что обозначает директива USER 1000, в файле Dockerfile  
UnionFS  
Что выдаст команда id, запущенная в контейнере  
docker uid remapping  

Dockerfile:  
    - ENV vs ARG  
    - ADD vs COPY  
    - CMD vs ENRTYPOINT  
    - EXPOSE  
Best practices:  
    - development  
    - dockerfile  
    - security  
Docker compose:  
    - depends_on

---

### DB

## Postgresql
Как вывести список активных соединений на Postgresql  
Что такое WAL  
Максимальный размер таблицы  
Хранение бинарных данных  
Как организован кластер  
Patroni - что это и зачем  
SQL:  
    - COUNT  
    - AVG  
    - SUM  
    - INNER JOIN  
    - LEFT JOIN  
    - RIGHT JOIN  
    - OUTTER  
    - HAVING VS WHERE  
    - DISTINCT  
    - Индекс, алгоритм индекса  

---

### Python

Передавать аргументы в командной строке  
Структуры и типы данных  
list vs tuple  
Аннотации  
Очереди - deque  
Менеджер контекста  
Работа с  JSON  
Механизм интернирования(256, 257)  
try/expect/finally  
assert  
lambda
if __name__ == “__main__”:  
*args or  **kwargs
yield
Decorators
Как передать переменную из одной функции в другую python  
Classes:  
    - как наследовать
    - _Some  
    - __Some

---

### Terraform

Импорт существующих ресурсов  
Можно ли править вручную tfstate  
Cloud-Init  

---
	
### Kafka

Для чего нужны брокеры сообщений  
Зачем много партиций в топике (производительность)  
Зачем нужна репликация (надежность)  

---

### Helm  

Для чего нужен файл _helpers.tpl  

---

##### *Мои вопросы*

Расскажите подробнее про проект?  
Какой технологический стек?  
Где находится/разворачиватся инфраструктура?  
Есть ли Legacy на проекте?  
Расскажите о команде?  
Сколько уже ДевоПсов на проекте?  
По какой методологии работаете?  
Как часто релизы?  
Есть ли процессы импортозамещения?  
Сколько и какие этапы собеседования?  
Можете дать какие-нибудь советы или материалы по подготовке к собеседованию?  
Как я буду оформлен?  
Какой формат работы?  
Есть ли ограничени по часовому поясу?  
Можно ли работать вне РФ?  
Выдаете ли оборудование, если да, то какое?  
Выделяются ли деньги на оборудование удаленного рабочего места?  
Есть ли Welcome бонус, премии, компенсация за оборудования для удаленного рабочего места?  
Какой грейд?  
Какая вилка у грейда?  
Есть ли пересмотр ЗП, если да, как часто?  
Какая должность(формулировка)?
Есть ли перспективы роста(горизонтальные/вертикальные)?  
Есть ли командировки?  
Есть ли дежурства?  
Придется работать в выходные, если да, это оплачивается?  
Придется ли задерживаться после 18-00?  
Есть ли медстраховка, компенсация спорта, обучение, сертификация и тд?  
Идеальный кандидат, какой он для вас?  
Чем предстоит заниматься сразу после найма и онбординга?  
Для чего вы нанимаете нового сотрудника(расширение команды, замена, новый функционал)?  
Когда ждать фидбек и в каком виде он будет?  