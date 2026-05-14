# Clínica Pets

Sistema simples de gestão para clínica veterinária desenvolvido em Java com integração ao banco de dados MySQL.

---

## Estrutura do Projeto

```bash
clinica-pets/
├── banco.sql                  # Rode PRIMEIRO no MySQL
├── pom.xml                    # Maven com driver MySQL 8.3
├── README.md
└── src/main/
    ├── resources/
    │   └── banco.properties 
    └── java/com/clinica/
        ├── model/             # Tutor · Pet · Consulta
        ├── dao/               # ConexaoDB · TutorDAO · PetDAO · ConsultaDAO
        └── ui/
            └── Menu.java      # Entry point (menu de console)
