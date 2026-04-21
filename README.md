# CadastroDeNinjas
mvn clean install

Configuração
Clone o repositório: git clone https://github.com/horaciomuller/CadastroDeNinjas.git
Navegue até o diretório do projeto: cd CadastroDeNinjas
Construa o projeto: mvn clean install
Execute a aplicação: mvn spring-boot:run
Acesse a aplicação em http://localhost:8080

Caso você não use o intellij onde você informa as variáveis de ambiente nas configurações, ao utilizar 
o maven:

Variável precisa estar no ambiente ou via -D
Maven só entra nisso se você configurar filtering (geralmente não vale a pena)
Exemplo:
java -DDATABASE_URL=jdbc:postgresql://localhost:5432/meubanco -jar target/app.jar
ou
$env:DATABASE_URL="jdbc:postgresql://localhost:5432/meubanco"
e rode o mvn em seguida