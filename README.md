# Exercicio: arquivos duplicados

### Descrição

Neste exercício, você utilizará a API (https://docs.oracle.com/javase/7/docs/api/) de 
arquivos do Java. O objetivo é varrer todos os arquivos existentes em um diretório 
informado via linha de commando. 

Por exemplo, ao executar o seguinte comando:  
```
java -jar target/app.jar /home/downloads/
```
o programa deverá imprimir na tela algo como:
```
[ /home/downloads/Exercício 03.docx - /home/downloads/Exercício 03 (1).docx ]
[ /home/downloads/foto1.jpg - /home/downloads/foto33.jpg - /home/downloads/foto12 (1).jpg ]
```

Orientações para entrega:
- Seu projeto deve ser um projeto maven válido, i.e., `mvn clean package` deve produzir 
um executável chamado `target/<seu-projeto>.jar`
