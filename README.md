# Exercicio: listar arquivos duplicados

**NOME**: seu_nome_aqui

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
Exercício 03.docx
Exercício 03 (1).docx 
foto1.jpg
foto33.jpg
foto12 (1).jpg 
```

## Critérios para definição de igualdade de arquivos:
- Mesmo conteúdo ([Files.readAllBytes](https://docs.oracle.com/javase/8/docs/api/java/nio/file/Files.html#readAllBytes-java.nio.file.Path-))
- Mesma data de modificação ([Files.getLastModifiedTime](https://docs.oracle.com/javase/8/docs/api/java/nio/file/Files.html#getLastModifiedTime-java.nio.file.Path-java.nio.file.LinkOption...-))
- Mesmo tamanho ([File.length](https://docs.oracle.com/javase/8/docs/api/java/io/File.html#length--))

## Orientações para entrega:
- Seu projeto deve ser um projeto maven válido, i.e., `mvn clean package` deve produzir 
um executável chamado `java -jar target/<seu-projeto>.jar`
