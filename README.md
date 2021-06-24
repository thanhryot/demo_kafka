# Demo kafka php


### Cách sử dụng:
- Bước 1: Yêu cầu có module rdkafka (php -m).
- Bước 2: Tải apache kafka theo link sau và start môi trường:
  https://www.apache.org/dyn/closer.cgi?path=/kafka/2.8.0/kafka_2.13-2.8.0.tgz
  
```

# Exact file and go to folder
tar -xzf kafka_2.13-2.8.0.tgz
cd kafka_2.13-2.8.0
  
  
# Start the ZooKeeper service (yêu cầu java 8+)
bin/zookeeper-server-start.sh config/zookeeper.properties
  
# Start the Kafka broker service
bin/kafka-server-start.sh config/server.properties 
  
```

- Bước 3: Từ thư mục mở terminal chạy:
```
php producer.php
```

Từ terminal khác chạy
```
php consumer.php
```
Test: Nhập nội dung thay đổi bên terminal producer và xem kết quả bên consumer.
