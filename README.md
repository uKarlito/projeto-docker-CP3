#Estrutura do projeto

clinica-pets/
├── banco.sql                  ← Rode PRIMEIRO no MySQL
├── pom.xml                    ← Maven com driver MySQL 8.3
├── README.md
└── src/main/
    ├── resources/
    │   └── banco.properties   ← Coloque suas credenciais aqui
    └── java/com/clinica/
        ├── model/             Tutor · Pet · Consulta
        ├── dao/               ConexaoDB · TutorDAO · PetDAO · ConsultaDAO
        └── ui/
            └── Menu.java      ← Entry point (menu de console)

#Como rodar

1. Criar o banco:
bashmysql -u root -p < banco.sql
2. Editar as credenciais em src/main/resources/banco.properties:
propertiesdb.url=jdbc:mysql://localhost:3306/clinica_pets?...
db.usuario=root
db.senha=SUA_SENHA
3. Compilar e rodar:
bashmvn package
java -jar target/clinica-pets.jar

#O que o sistema faz
MóduloOperaçõesTutoresListar, Cadastrar, Editar, ExcluirPetsListar todos, Listar por tutor, Cadastrar, Editar, ExcluirConsultasListar todas, Histórico por pet, Registrar, Excluir
