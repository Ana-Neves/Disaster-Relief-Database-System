![imagem para ilustração](assets/readme/banner.jpg)

# Relief and Support Portal (RSP)

## 📌 Organization Description

The **Relief and Support Portal (RSP)** is an innovative and integrated platform, conceived in response to recent disasters in Rio Grande do Sul. It is dedicated to providing fast and effective assistance to people in vulnerable situations, especially during natural disasters such as floods, earthquakes, fires, and other emergencies.

Developed to streamline resource management and coordinate humanitarian aid, the RSP aims to connect donors, volunteers, and support organizations in order to maximize the impact of relief efforts.

## 🎯 Mission

The RSP’s mission is to save lives and alleviate the suffering of people affected by disasters by promoting solidarity and community cooperation.

The platform serves as a central hub for support, ensuring that vital resources quickly reach those who need them most, while keeping relief efforts efficient and transparent.

> With the RSP, we turn solidarity into action—building a strong and effective support network in times of crisis.

## 🧩 Project Organization

To ensure efficiency and transparency, our team adopted collaborative tools and workflows:

- **Trello & Notion**
  - Trello was used for task management and progress tracking.
  - Notion was used to document requirements, diagrams, and design decisions.

![Trello Board](assets/readme/trello.png)

- **Discord Meetings**
  - Regular meetings were held via Discord to align strategies, track progress, and resolve issues.

- **Live Share (VS Code)**
  - Used for real-time collaborative coding, code reviews, and problem-solving.

These practices improved organization, communication, and overall team productivity.

## 🏗️ Project Structure

### 📊 Diagrams

- **Conceptual Diagram** – High-level representation of entities and relationships  
- **Logical Diagram** – Detailed database structure (tables, columns, data types, relationships)

### 🗄️ Database

- **MySQL Workbench** – Database creation and management  
- **SQL Script** – Includes:
  - Database and table creation
  - Sample data insertion
  - Basic queries

## ⚙️ How to Use

### 📋 Prerequisites

- [MySQL](https://www.mysql.com/downloads/)
- [MySQL Workbench](https://www.mysql.com/products/workbench/)

### 🚀 Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/Kerubink/Projeto-M3---PDA-.git
   cd your-repository
   
2. **Open MySQL Workbench**

   - Connect to your MySQL server
     
3. **Import SQL Script**

  - Go to File `File` > `Open SQL Script` e selecione o arquivo `database_script.sql` localizado no repositório clonado.

   > `Para mais informações acesse o arquivo de instruções na pasta MySQL`
   >
4. **Execute the Script**

- Execute the SQL script to create the database and the necessary tables.

### Test Queries

After importing and running the SQL script, you can perform some test queries to ensure the database has been configured correctly. You can find more example queries in the file. `INSTRUCTIONS.md`.

```sql
-- Exemplo de consulta para verificar dados inseridos em uma tabela
SELECT * FROM Agua_Potavel;

-- Exemplo de consulta para verificar o relacionamento entre tabelas
SELECT *
FROM Doacao d
JOIN Usuarios u ON d.UsuarioID = u.ID_Usuarios
JOIN Instituicao i ON d.InstituicaoID = i.ID_Instituicao;
```

## Database Structure

### Some tables in our database

- **Drinking_Water**

  - `ID_Agua`: Unique identifier.
  - `Volume`: Volume in liters.
  - `Data_de_Validade`: Packaging expiration date.
  - `Nivel_de_Urgencia`: Level of urgency (1 - Low, 2 - Medium, 3 - High).
  - `Embalagem`: Packaging type.
  - `Descricao`: Description of drinking water.
  - `Fornecedor`: Supplier's name.
    
- **Food**
  
  - `ID_Alimentos`: Unique identifier.
  - `Nome`: Name of the food.
  - `Categoria`: Food category.
  - `Data_de_Validade`: Food expiration date.
  - `Quantidade`: Quantity in kilograms.
  - `Descricao`: Food description.
  - `Nivel_de_Urgencia`: Level of urgency. (1 - Low, 2 - Medium, 3 - High).
  - `Fornecedor`: Supplier's name.
    
- **Users**
  - `ID_Usuarios`: Unique identifier.
 - `Username`: User's name.
- `Email`: User's email (unique).
- `Address`: User's address.
- `UserType`: User type.
- `Institution_ID`: Identifier of the associated institution.
  
- **Institution**
- `ID_Institution`: Unique identifier.
- `Institution_Name`: Institution name.
- `Email`: Institution email.
- `Phone`: Institution phone number.
- `Addresses`: Institution address.
- `Description`: Institution description.
  
- **Voluntarios**

  - `ID_Voluntario`: Identificador único.
  - `Nome_Voluntario`: Nome do voluntário.
  - `Disponibilidade`: Disponibilidade do voluntário.
  - `Habilidades`: Habilidades do voluntário.
  - `Email`: Email do voluntário.
  - `Telefone`: Telefone do voluntário.
  - `Descricao`: Descrição do voluntário.

### Relationships

- **Donation**: Relates users, institutions, and donated items (water, food, clothing, etc.).
- **Volunteer_Institution**: Relates institutions and volunteers.
- **Assistance_Institution**: Relates institutions and technical assistance.
- **Institution_User**: Relates users and institutions.

## Conclusion

This project provided a deeper understanding of database modeling and practical implementation using MySQL. We appreciate the opportunity to apply the knowledge and skills we acquired throughout the course. If you encounter any problems or have questions, feel free to open an issue in the repository or contact any of the contributors.

## Contributors


### Leader


![Kauã](https://avatars.githubusercontent.com/u/112822162?v=4)
**Kauã Kelvyn**
Desenvolvedor Fullstack - Líder

- GitHub: [Kerubink](https://github.com/Kerubink)
- LinkedIn: [Kauã Kelvyn](https://www.linkedin.com/in/kau%C3%A3-moraes-079288303/)

### Comunicator


![Samuel](https://avatars.githubusercontent.com/u/105753686?v=4)
**Samuel**
Desenvolvedor Fullstack - Communications

- GitHub: [Samuel-Kepler](https://github.com/Samuel-Kepler)
- LinkedIn: [Samuel](https://www.linkedin.com/in/samuel-ribeiro-loiola)

### Knowledge Manager


![Miszael](https://avatars.githubusercontent.com/u/119391809?v=4)
**Miszael**
Desenvolvedor Fullstack - Knowledge Manager

- GitHub: [minu1123](https://github.com/minu1123)
- LinkedIn: [Miszael](https://www.linkedin.com/in/miszael-costa-19b0b4251/)

### Contributors


![Ana](https://avatars.githubusercontent.com/u/97240075?v=4)
**Ana Caroline Neves**
Fullstack Developer - Colaboradora

- GitHub: [Ana-Neves](https://github.com/Ana-Neves)
- LinkedIn: [Ana](https://www.linkedin.com/in/ana-caroline-neves-fullstack/)


![Beatriz](https://avatars.githubusercontent.com/u/141242413?v=4)
**Beatriz**
Fullstack Developer - Colaboradora

- GitHub: [l1Beatriz](https://github.com/l1Beatriz)
- LinkedIn: [Beatriz](https://www.linkedin.com/in/beatrizsantos009?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)
