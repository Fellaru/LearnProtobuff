Это учебный проект по теме  protobuf
Выполняю по вот этому tutorial: https://developers.google.com/protocol-buffers/docs/javatutorial

Как начать:
1. Создайте .proto файл с описанием структуры данных. Я сделала src/main/java/AddressBook.proto. Вы найдете полное руководство по написанию .proto файлов, включая все возможные типы полей, в [Protocol Buffer Language Guide](https://developers.google.com/protocol-buffers/docs/proto)
1. Установить proto компилятор и скомпилировать ваш .proto файл. Соответвтсвующая глава из [туториала](https://developers.google.com/protocol-buffers/docs/javatutorial)
Для mac ```brew install protobuf``` 
1. Проверте что proto компилятор установлен ```protoc --version```
1. Зайдите в директорию, где лежит ваш .proto файл 
1. Выполните ```protoc --java_out=.  AddresBook.proto```, 
1. Добавьте в pom необходимые зависимости  и проверте сборку с помощью ```mvn compile```
``` 
    <dependencies>
        <dependency>
            <groupId>com.google.protobuf</groupId>
            <artifactId>protobuf-java</artifactId>
            <version>3.11.4</version>
        </dependency>
    </dependencies>
```

